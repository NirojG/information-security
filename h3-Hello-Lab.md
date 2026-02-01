# h3 - Hello Lab 
## x) Installation of Debian on Virtualbox - Karvinen 2021 (Updated 2024)
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

- I pinged cloudfare ip while the internet is connected. I used command ping 1.1.1.1 in terminal and killed the ping by using ctrl + c. 
<img width="1287" height="807" alt="image" src="https://github.com/user-attachments/assets/34147b72-be31-490b-a88f-415f4f65e8b3" />

- I disabled the network on my virtual box and tried pinging both cloudfare and google DNS and observed the network was unreachable. Below is the screenshot for the task performed on my linux.
 <img width="1286" height="802" alt="image" src="https://github.com/user-attachments/assets/91263339-4f30-4447-82b1-44a5bfd73063" />

## b) Portscan local only 
- first we need to install nmap in our system, we have to open terminal and execute sudo apt-get install nmap, we can scan our own local host using sudo nmap -A localhost.
- I port scanned using nmap to see what ports are open on our own system while the internet is still off. It is illegal to portscan so, I made sure to keep my internet off through out its usage.

<img width="1282" height="797" alt="image" src="https://github.com/user-attachments/assets/cec8a2b3-121b-4111-8c68-84bed38a1427" />

- I obsereved there is only one IP address which is scanned and this is to be expected.

## c) Daemon scan
- I Installed apache by executing sudo apt-get -y install apache2.
- I also started the daemon sudo systemctl start apache2.
- I run the nmap command again sudo nmap -A localhost below is the result of nmap scan.
- now we can observe port 80 is open!
  
<img width="1281" height="802" alt="image" src="https://github.com/user-attachments/assets/7ccaf628-4ed4-43ab-98c4-e6bc1b3c3755" />

## d) Bandit oh-five 
- Firstly I installed the ssh through this command in terminal sudo apt-get install openssh-client.
- I connected to the over the wire  Bandit wargame. First level started from level 0 where i had to connect to their server.
- I used ssh bandit0@ bandit.labs.overthewire.org to connect my username based game.
- I used password given bandit0 to login. Below is the screenshot of my work. This is the task for Level0
  
<img width="827" height="532" alt="image" src="https://github.com/user-attachments/assets/6ab668cc-0748-4941-8992-e9e6da589d11" />

### From level 0 to 1
- the password is in readme file to locate it I used "ls" in terminal to showcase the files.
- I used cat readme to read the content and from that I located the password.
  
<img width="1280" height="797" alt="image" src="https://github.com/user-attachments/assets/2f46c152-fcfd-4366-a6e1-6ca0379b7410" />

### From level 1 to 2
- I logged in as bandit1 user and entered the password through ssh bandit1@bandit.labs.overthewire.org -p 2220.
  
<img width="1281" height="790" alt="image" src="https://github.com/user-attachments/assets/4b87e547-ac16-41a7-8a89-7eda53d402b3" />

- I used cat ./- to locate another password
  
<img width="822" height="397" alt="image" src="https://github.com/user-attachments/assets/2a5d7649-bf94-48d6-997f-79fed56408ac" />


### From level 2 to 3
- Now in the next task I have to login by bandit2 username and enter the password I got from above procedure.
- I used various techniques and finally located the password and exited bandit2 to reach the bandit3 user.
  
<img width="1275" height="588" alt="image" src="https://github.com/user-attachments/assets/195ada87-4133-450d-99de-2a66813d9d72" />

- here i logged in bandit 3
  
<img width="1280" height="803" alt="image" src="https://github.com/user-attachments/assets/0fee2fb9-b946-4a0d-94fb-bbf008c6282a" />

### From level 3 to 4
- Now I tried various ways and finally got what i should be doing first we should cd inhere, and to find the files i used ls -a and i located the file and the password.
  
<img width="1277" height="792" alt="image" src="https://github.com/user-attachments/assets/cccc0d49-abc1-46d5-93be-783db07a0582" />

### From Level 4 to 5
- Now here I logged in to the bandit 4 and started searching for the files from the cd inhere directory, and the password for level 5 was in file 007.
  
<img width="1288" height="805" alt="image" src="https://github.com/user-attachments/assets/014695c7-132b-476f-b89c-02c729910de9" />

- After completion of all levels I logged in to bandit 5 and started doing some challange of this too. 

<img width="1277" height="796" alt="image" src="https://github.com/user-attachments/assets/9e3b17ea-cedd-4f90-9e9f-152ef83aa3e9" />


# Sources 
- Karvinen, T. 2021: Install Debian on Virtualbox - Updated 2024. Available at: https://terokarvinen.com/2021/install-debian-on-virtualbox/
- Karvinen, T. 2020: Command Line Basics Revisited. Available at: https://terokarvinen.com/2020/command-line-basics-revisited/
- OverTheWire Community: Bandit Wargame (Levels 0-34). Available at: https://overthewire.org/wargames/bandit/.

 
