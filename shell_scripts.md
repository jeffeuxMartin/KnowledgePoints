# Shell scripts

## prompt

Rel.: https://blog.devgenius.io/how-to-customize-the-git-bash-shell-prompt-336f6aefcf3f
<!-- Rel. = related resources -->

#### Open file system GUI on different OS systems
* Windows: `explorer $DIRNAME`
* MacOS: `open $DIRNAME`
* Linux: `xdg-open $DIRNAME`

```sh=
PS1='\[\033]0;$TITLEPREFIX:$PWD\007\]' # set window title
PS1="$PS1"'\n'                 # new line
PS1="$PS1"'\[\033[32m\]'       # change to green
PS1="$PS1"'\u@\h '             # user@host<space>
PS1="$PS1"'\[\033[35m\]'       # change to purple
PS1="$PS1"'$MSYSTEM '          # show MSYSTEM
PS1="$PS1"'\[\033[33m\]'       # change to brownish yellow
PS1="$PS1"'\w'                 # current working directory
PS1="$PS1"'\[\033[0m\]'        # change color
PS1="$PS1"'\n'                 # new line
PS1="$PS1"'$ '                 # prompt: always $
```
