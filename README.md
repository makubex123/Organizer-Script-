# Organizer-Script- :pizza:

This script helps to organize all your files in the Downloads Directory, and to distribute them to the respective directory, I hope you like it 

#First verify if the directory exist if not it will create it :)

test ! -d /home/$USER/Documents && mkdir /home/$USER/Documents 

test ! -d /home/$USER/Videos && mkdir /home/$USER/Videos 

test ! -d /home/$USER/Music && mkdir /home/$USER/Music 

test ! -d /home/$USER/Pictures && mkdir /home/$USER/Pictures  

test ! -d /home/$USER/archivos && mkdir /home/$USER/archivos

#Then after create the directory will execute the transfer of the files

mv /home/$USER/Downloads/{*.doc,*.docx,*.pdf,*.odt,*.abw} /home/$USER/Documents

mv /home/$USER/Downloads/{*.mp4,*.flv,*.avi,*.mkv} /home/$USER/Videos

mv /home/$USER/Downloads/{*.mp3,*.wav,*.ogg,*.wma} /home/$USER/Music

mv /home/$USER/Downloads/{*.png,*.jpg,*.gif} /home/$USER/Pictures

mv /home/$USER/Downloads/{*.iso,*.deb,*.rpm,*.zip,*.rar,*.sh,*.tar,*.bz2} /home/$USER/archivos

#Please notice that the name of the directories are in English if your distro is in another language please change their name
