## termux arch setlocale UTF-8

https://github.com/sdrausty/TermuxArch/issues/117

```bash

[root09:21home]$cat /root/.bash_profile
if [ ! -e "$HOME"/.hushlogin ] && [ ! -e "$HOME"/.chushlogin ] ; then
. /etc/motd
fi
if [ -e "$HOME"/.chushlogin ] ; then
rm "$HOME"/.chushlogin
fi
PATH="$HOME/bin:$PATH"
. "$HOME"/.bashrc
PS1="[\e[38;5;148m\]\u\[\e[1;0m\]\A\[\e[1;38;5;112m\]\W\[\e[0m\]]\$"
# PS1="[\A\[\033[0;32m\] \W \[\033[0m\]]\$ "
export TZ="America/New_York"
export LANG="en_US.UTF-8"
export LANGUAGE="en_US.UTF-8"
export LC_ADDRESS="en_US.UTF-8"
export LC_COLLATE="en_US.UTF-8"
export LC_CTYPE="en_US.UTF-8"
export LC_IDENTIFICATION="en_US.UTF-8"
export LC_MEASUREMENT="en_US.UTF-8"
export LC_MESSAGES="en_US.UTF-8"
export LC_MONETARY="en_US.UTF-8"
export LC_NAME="en_US.UTF-8"
export LC_NUMERIC="en_US.UTF-8"
export LC_PAPER="en_US.UTF-8"
export LC_TELEPHONE="en_US.UTF-8"
export LC_TIME="en_US.UTF-8"

[root09:23home]$cat /etc/locale.conf
##  File locale.conf generated by setupTermuxArch.sh at 20180913205526.
LANG=en_US.UTF-8
LANGUAGE=en_US.UTF-8
LC_ADDRESS=en_US.UTF-8
LC_COLLATE=en_US.UTF-8
LC_CTYPE=en_US.UTF-8
LC_IDENTIFICATION=en_US.UTF-8
LC_MEASUREMENT=en_US.UTF-8
LC_MESSAGES=en_US.UTF-8
LC_MONETARY=en_US.UTF-8
LC_NAME=en_US.UTF-8
LC_NUMERIC=en_US.UTF-8
LC_PAPER=en_US.UTF-8
LC_TELEPHONE=en_US.UTF-8
LC_TIME=en_US.UTF-8

```
