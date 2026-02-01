# h3 - Hello Lab 
## Installation of Debian on Virtualbox - Karvinen 2021 (Updated 2024)
- First downloading the image , debian ISO image latest version.
- Downloading & installing virtual box.
- Creating New virtual machine of debian.
- create virtual hard disk drive.
- boot the image, while unselecting unattended installation (which usually is not good) and choose the live version installation.
- run the debain installer and choose good password.
- sudo means superuser priveliage in linux.
- for getting the latest update of the debian using CLI and inserting sudo -apt-get -update and hiting the return key.
- sudo apt-get -y dist-upgrade where, "-y" says yes to stupid questions. "dist-upgrade" means upgrade everything. It installs the latest versions of all software.

## Karvinen 2020: Command Line Basics Revisited
### Moving and looking around 
- 'pwd' prints the working directory.
- ls lists file in the working directory.
- cd terosdir/ means change directory to terosdir.
- cd.. moves the directory to one level up.
- less tero.txt, opens the file to read 
- ls/ etc | less, scrolls long command output page by page.

### File Manipulations in Linux 
- Easiest text editors are pico and nano.
- nano Foo.txt, This is creation of simple terminal txt editor.
- to create a directory mkdir Newfolder
- move/ rename a folder mv oldname newname, mv filename.txt NEWDIR/
- cp -r ORIGINAL COPY, this copies original to -r meaning recursive.
- rmdir remove an empty directory.
- rm junk removes junk.
- rm -r FOLDEROFJUNK this removes the FOLDEROFJUNK without any warnings.

### SSH Remote Control 
- ssh tero@example.com Opens a remote command shell in a very secure way. Here, username is tero and server is example.com.
- Exit back to your own machine with ‘exit’ remotecomputer$ exit

### Help 
- to show the manual page of a command man ls
- ls --help, this offers quick help.
- ctrl + R reverse search previous commands.
- ls /etc/resolve.[TAB] this autocompletes filenames and commands.

### Important system directories 
- / - Root of the file system
- /home/username - User's personal files
- /etc/ - System configuration files
- /var/log/ - System logs
- /media/ - USB drives, CDs, etc.

## a) can't fish 
- I disabled the network on my virtual box and tried pinging both cloudfare and google DNS and observed the network was unreachable. Below is the screenshot for the task i did
- <img width="1286" height="802" alt="image" src="https://github.com/user-attachments/assets/91263339-4f30-4447-82b1-44a5bfd73063" />
- 

