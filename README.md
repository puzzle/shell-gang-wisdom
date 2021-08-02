# shell-gang-wisdom

Neat oneliners and tricks gathered from day to day shell work at puzzle.

# Are you a Puzzle member?

Visit the channel `#shell-gang` to meet the gang. If you're not yet a Puzzle member, [join us](https://www.puzzle.ch/de/ueber-uns/stellen).

# Aliases
Did you find a cool one-liner? Instead of writing it down in your notebook, why not create an alias? These can be added to `~/.bashrc` or `~/.zshrc`, depending if you are using Bash or Zsh. You can load the aliases by opening a new terminal or running `source ~/.bashrc`. Execute `alias` anytime to get a list of all your aliases.

## Copy process output to clipboard
```
alias copy='ruby -e "print readlines.join.chomp" | xclip -sel clip'
```
and use it like `pwd | copy`.

## Easier parent directory navigation
```
alias ..='cd ..'
alias ...='cd ../..'
```

# Bash Tricks

## Get the previous commands last argument
example:
```
$ mkdir ~/.ssh
$ chmod 0700 !$
```
## Rerun the last command
example:
```
$ apt install cowsay
$ sudo !!
```
