A simple terminal + vim environment for recording on-line training video.

## Terminal

Use terminal.app at Mac OS.

## Shell

Use bash shell with a simple ```~./.bashrc```.

```
# set a fancy prompt (non-color, unless we know we "want" color)
case "$TERM" in
    xterm-color) color_prompt=yes;;
esac
color_prompt=yes

if [ "$color_prompt" = yes ]; then
    PS1='${debian_chroot:+($debian_chroot)}\[\033[01;33m\]\u\[\033[37m\]@\[\033[32m\]local\[\033[37m\]:\[\033[31m\]\w \[\033[36m\]\$\[\033[00m\] '
    #PS1='${debian_chroot:+($debian_chroot)}\[\033[01;33m\]\u\[\033[37m\]:\[\033[31m\]\w \[\033[36m\]\$\[\033[00m\] '
else
    PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w\$ '
fi
```

## vim

Use vim with a simple ```~./.vimrc```.

```
set nocompatible
" force 256 colors on the terminal
set t_Co=256
set number
set cursorline
syntax on
hi CursorLine   cterm=NONE ctermbg=254 ctermfg=NONE
```

## font

Use [Source Code Pro](https://github.com/adobe-fonts/source-code-pro) from Adobe.
