# .bashrc



## Custom commands
``` bash
# Variable shortcut to repository/projects folder
export REP="/home/USER/Documents/repositories"
# "~" in variables will fail when used with cd (eg: cd $REP)
function rep(){ command cd $REP; }

# Functions to execute some programs/scripts straight from CLI
# Functions over alias (alias can't be exported so they can't be used inside session scripts)
function gdrive(){ $REP/third/gdrive $@; }
function sws(){ ~/.scripts/start_workspace.sh $@; }

# Export functions so they are available from session scripts
export -f rep gdrive

# Set history size to 5k and filesize to 10kb
# bc i want my entries to be available for reverse-i-search
HISTSIZE=5000
HISTFILESIZE=10000
```
