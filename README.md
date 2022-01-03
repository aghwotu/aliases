# aliases

My personal aliases. You will notice that sometimes there are two aliases for the same command. I do this because sometimes I remember one and forget the other so I have them both depending on whichever one I remember.

# Recommendation

My personal rule for aliases is that they can be as long or as short as you want them to be as long they help you to be more efficient.

# Adding aliases to your terminal

I LOVE using aliases and for Windows I use the '[cmder](https://cmder.net/)' terminal and on macOS I use '[iTerm](https://iterm2.com/index.html)' and '[zsh](https://ohmyz.sh/)'. I saw a neat trick today - May, 15 2021. Add the path to your alias file as an alias.

I use VSCode and my alias file on Windows is at `C:/tools/cmder/config/user_aliases.cmd`. Now, create a new alias called `add_alias` and add it to your alias file like so:

```bash
add_alias= code /tools/cmder/config/user_aliases.cmd
```

Now, whenever you type `add_alias` in your terminal, it would open your `user_aliases.cmd` file in VSCode and you can add your new aliases.

> **NOTICE**: Please take note of the differences between the syntax for the macOS and Windows aliases.

### macOS alias syntax

```bash
alias cl="clear"
```

### Windows alias syntax

```bash
cl=clear
```

# System - macOS only

```bash
alias add_alias="code ~/.zshrc"
alias add_new_alias="code ~/.zshrc"
alias cl="clear"
alias new_alias="code ~/.zshrc"
alias show_variables="printenv"
```

# System - Windows only

```bash
cl=clear
e.=explorer .
add_new_alias= code /tools/cmder/config/user_aliases.cmd
add_alias= code /tools/cmder/config/user_aliases.cmd
new_alias= code /tools/cmder/config/user_aliases.cmd
gocode=cd C:\code
codefiles=cd C:\code
root=cd C:\
```

# Laravel - macOS

```bash
alias art="php artisan"
alias server="php artisan serve"
alias tinker="php artisan tinker"
```

# Laravel - Windows

```bash
art=php artisan $*
server=php artisan serve
tinker=php artisan tinker
```

# Git - macOS

```bash
alias gs="git status"
alias gc="git commit"
alias grab="git branch -a"
alias gp="git push origin master"
alias gl="git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
alias gd="git diff"
alias git_edit_origin="git remote set-url origin"
alias git_add_origin="git remote add origin"
alias grab_all_branches="git remote update"
alias grab_remote_branches="git remote update"
alias gcl="git clone"
```

# Git - Windows

```bash
ga=git add $*
gc=git commit $*
gcl=git clone $*
gs=git status
grab=git branch -a
git_edit_origin=git remote set-url origin $*
git_add_origin=git remote add origin $*
grab_all_branches=git remote update
grab_remote_branches=git remote update
```

# MongoDB - macOS only

```bash
alias start_mongo="brew services start mongodb-community@5.0"
alias mongo_start="brew services start mongodb-community@5.0"
alias stop_mongo="brew services stop mongodb-community@5.0"
alias mongo_stop="brew services stop mongodb-community@5.0"
alias end_mongo="brew services stop mongodb-community@5.0"
alias mongo_config="code /System/Volumes/Data/opt/homebrew/etc/mongod.conf"
```
