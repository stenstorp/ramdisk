# Ramdisk and Ramdisk-cleanup
Easily create and remove ramdisks for files and folders seamlessly on Linux

Ramdisk-cleanup removes selected ramdisk/s, restoring the original file structure


## Ramdisk

Ramdisk puts the selected files and folders into ram while allowing any program to use them as if they had not been moved.
Ramdisks are created with exactly enough space to put the selected files into with 1MB of breathing room by default.

USAGE: \
ramdisk [PATH] [BUFFER] \
PATH: The path to the folder/files you want to put into the ramdisk \
BUFFER: Extra space in the ramdisk in Megabytes (Default 1)

EXAMPLE: \
ramdisk /home/user/Games/FunGame 150 \
This will put "FunGame" into a ramdisk with 150MB of free space to account for file growth. eg, save files.


## Ramdisk-cleanup

Ramdisk-cleanup removes selected ramdisk/s, restoring the original file structure.

USAGE: \
ramdisk-cleanup (NAME)
NAME: Name of the ramdisk to clean 

You will be prompted to type/copy the name of the ramdisk you want to remove.

## Installation instructions
clone the repository:\
git clone https://github.com/stenstorp/ramdisk.git

Make them executable:\
chmod +x ramdisk/ramdisk*

Move/copy files to somewhere in your $PATH eg:\
cp ramdisk/ramdisk* ~/.local/bin
