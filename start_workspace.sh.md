# Start My Workspace

### Backup Notes-Up DB
#### `nosync` to prevent execution
	if [[ ! "$@" == *"nosync"* ]]; then
		gdrive sync upload --keep-local ~/.local/share/notes-up GD_FOLDER_ID
	fi

### Start DB service
	sudo service mysql start

### Open browser (WhatsApp Web, Discord, YTMusic)
##### `nowsp` or `nodc` or `nomusic` to prevent execution
	query="google-chrome"
	if [[ ! "$@" == *"nowsp"* ]]; then
		query+=" https://web.whatsapp.com/"
	fi
	if [[ ! "$@" == *"nodc"* ]]; then
		query+=" https://discord.com/app"
	fi
	if [[ ! "$@" == *"nomusic"* ]]; then
		query+=" https://music.youtube.com/watch?v=dUNOfNad59Q"
	fi
	if [ ! "$query" == "google-chrome" ]; then
	   $query --new-window &
	fi

### Open project
###### Uses [elementaryOS terminal](https://github.com/elementary/terminal)
	function exec(){ io.elementary.terminal -t -x "bash -c '$@'"; }

	# Some Project
	if [[ "$@" == *"keyword"* ]]; then
		echo "--- Project ---"
		exec \
			atom -n $REP/project
