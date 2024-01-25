# Git Aliases

## Script

* Run `git-alias-setup.sh`
* `chmod +x git-alias-setup.sh`
* `./git-alias-setup.sh`

## Manual Setup

```
$ git config --global alias.co checkout
$ git config --global alias.br branch
$ git config --global alias.ci commit
$ git config --global alias.st status
$ git config --global alias.unstage 'reset HEAD --'
$ git config --global alias.last 'log -1 HEAD'
```

## Usage

```
$ git co -b 'edvins/new-feature'
$ git br master
$ git ci -m 'Intial commit' 
$ git st
$ git unstage
$ git last
```
