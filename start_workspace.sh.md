# Start My Workspace
###### Requires to have defined variable REP
###### REP="~/Documents/repositories/" (i include it in .bashrc)


### Backup Notes-Up DB
	gdrive sync upload --keep-local ~/.local/share/notes-up 1oLl7K9wK93B1EZVkYLWhLvjeaenCK3Zy

### Start DB service
	sudo service mysql start

### Open browser (WhatsApp Web, Discord, YTMusic)
	google-chrome https://web.whatsapp.com/
	google-chrome https://discord.com/app
	google-chrome https://music.youtube.com/watch?v=dUNOfNad59Q


### Open project
###### Uses [elementaryOS terminal](https://github.com/elementary/terminal)
	if [ "$1" != "" ]; then
		if false; then true

		# Project1
		elif [ "$1" == "keyword1" ] || [ "$1" == "KEYWORD1" ]; then
			echo "--- Project1 ---"
			# Define pre defined function to execute per project
			#io.elementary.terminal -- COMMAND

		# Project2
		elif [ "$1" == "keyword2" ]; then
			echo "--- Project2 ---"

		fi
	fi
