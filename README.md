# shell-gang-wisdom

Neat oneliners and tricks gathered from day to day shell work at puzzle.

# Are you a Puzzle member?

Visit the channel `#shell-gang` to meet the gang. If you're not yet a Puzzle member, [join us](https://www.puzzle.ch/de/ueber-uns/stellen).

# Commands

## Copy process output to clipboard

Add this to your .bashrc

    alias copy='ruby -e "print readlines.join.chomp" | xclip -sel clip'

and use it like `pwd | copy`.

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
