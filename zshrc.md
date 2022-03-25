# Oh My ZSH settings

### `.zshrc` general

```
# To automate managing of the node version upon entering directories with .nvmrc files
autoload -U add-zsh-hook
load-nvmrc() {
  local node_version="$(nvm version)"
  local nvmrc_path="$(nvm_find_nvmrc)"

  if [ -n "$nvmrc_path" ]; then
    local nvmrc_node_version=$(nvm version "$(cat "${nvmrc_path}")")

    if [ "$nvmrc_node_version" = "N/A" ]; then
      nvm install
    elif [ "$nvmrc_node_version" != "$node_version" ]; then
      nvm use
    fi
  elif [ "$node_version" != "$(nvm version default)" ]; then
    echo "Reverting to nvm default version"
    nvm use default
  fi
}
add-zsh-hook chpwd load-nvmrc
load-nvmrc
```

### `.zshrc` work-related

```
# Workshop related aliases
alias ws-up="docker-compose -f ~/Documents/repos/services/workshop/docker-compose.yml up -d --force-recreate sedna platform nginx dynamodb-local search-platform"
alias ws-stop="docker-compose -f ~/Documents/repos/services/workshop/docker-compose.yml stop"
alias ws-down="docker-compose -f ~/Documents/repos/services/workshop/docker-compose.yml down"
alias ws-setup="~/Documents/repos/services/workshop/bin/setup-workshop.sh --tear-down-es y"

# Generate specific amount of new emails
function wsImport() {
  if [ "$1" = "nodocker" ]; then
    TO_INDEX="1"
  else
    if [ "$2" != "nodocker" ]; then
      echo "Starting Worker Docker container..."
      docker start sedna-worker
    fi
    TO_INDEX="${1:-1}"
  fi
  echo "Importing $TO_INDEX email(s)..."
  pushd ~/Documents/repos/services/one-off-scripts/bulk_eml_creation
  yarn run exec --toIndex=$TO_INDEX
  ../import_emls_into_test_environment/import-emls-to-test-env.sh workshop ./target
  popd
}
```
