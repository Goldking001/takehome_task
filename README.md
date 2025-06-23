# takehome_task

#a copy of my bash script

#!/bin/bash

#Create an organized folder if the folder does not exist
mkdir -p organized/txt
mkdir -p organized/sh
mkdir -p organized/log

#loop through all files in the current directory
for file in *;do
	case "$file" in
		*.txt) mv "$file" organized/txt/ ;;
		*.sh) mv "$file" organized/sh/ ;;
		*.log) mv "$file" organized/log/ ;;
	esac
done
