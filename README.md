**Change directory to the tests directory using absolute pathname**
- cd /home/altschool/tests

**Change directory to tests using relative pathname**
- cd tests

**Use echo command to create a file named fileA with text content 'Hello A'in the misc directory**
- echo 'Hello A' > ./misc/fileA

**Create an empty file named fileB in the misc directory.Populate the file with dummy content**
- echo "Sally" > ./misc/fileB

**Copy contents of fileA into fileC**
- cp misc/fileA misc/fileC

**Move contents of fileB into fileD**
- mv misc/fileB misc/fileD

**Create a tar archive called misc.tar for the contents of misc directory**
- tar -cvf misc.tar ./misx

**Compress the tar archive to create a misc.tar.gz**
- gzip misc.tar

**Create a user and force the user to change his/her password upon login**
- sudo adduser sally && sudo passwd --expire madu

**Lock a user's password**
- sudo passwd -S sally

**Create a user with no login shell**
- sudo adduser salamat --shell /usr/sbin/nologin
  
**Disable password based auth for ssh**
- sudo nano /etc/ssh/sshd_config
- Click enter and it opens file
- Check for line starting with 'PasswordAuthentication no'
- Click i to enter insert mode
- If the line is commented ,uncomment it
- Change the line to 'PasswordAuthentication no'
- Press ESC and save new changes by typing: wq!
- Restart ssh with 'sudo service ssh restart'
  

**Disable root login for ssh**
-sudo nano /etc/ssh/sshd_config
- Look for the line PermitRootLogin 
- Change the line to PermitRootLogin no
- Press ESC to save the new changes ,type wq!
- Restart the ssh service with sudo servive ssh restart



