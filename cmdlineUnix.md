# Command line cheetsheet

1. Copy a folder to a new folder: `cp -R -v <foldername> <destination>`
2. List all the hidden files with human readable bytes: `ls -l -a  -h` => `s -lah` 
3. Multiple commands: `<first command> | <second command> |...`
4. Readable output with cat: `cat <file name> | more`
5. Words with cat : `cat <file name> | wc -w`
6. Search pattern with cat: `cat <file name> | grep <search pattern>`
7. Save tree in a file : `tree > data.txt`
8. Append tree to an existing file `tree >> data.txt`
9. Zip a file : `gzip <file name>.tar `
10. Decompress zip file: `gzip -d <zip file name>.zip `
11. Create an archive file or tarball: `tar -cvf <new name of archive file>.tar <file to archive>`
12. Restore a deleted archive file: `tar -xvf <archive file name`
13. Create zip tar file: `tar -czvf <new name of zip tar file>.tgz  <folder to zip>`
- `c`: create archive
- `z`: zip
- `v`: verbose
- `f`: file name next to Zip file
14. Extend archive file: `tar -xzvf <tgz file>`
15. Create nested directories: `mkdir -p <dir1/dir2/dir3...>`
16. Change mode file permission:
- `chmod u+w <filename>`: add permission
- `chmod g-rw <filename>`: remove permission
-  `chmod u=rwx, go=r <filename>`: set permission
-  `chmod a+rwx <filename>`: add permission to all
17. Change mode directory permission: 
- `chmod -R o-rwx <directoryname>`: remove permission recursively from others
- `chmod -R g+rwx <directoryname>`: add persmission rescursively to group
- `chmod -R a+rwx <directoryname>`: add permission recursively to all
18. Change group of file: `chgrp <new groupname> <file>`
19. Change owner of file: `sudo chown <new ownername> <file> `
20. `uname -a`: get information of your operating system

* * *
# Unix operating system

1. `ssh <host name>`: access remote host  e.g. `ssh 10.0.1.26` or `ssh web.de`
2. `sftp <remote server name>`: secure file transfer
- `put <filename>`: upload file to local machine
- `get <filename>`: downlad file from local machine 
- `exit`: exit secure file transfer
3. `scp [source] [destination]`: secure copy file to remote host
- `scp file.txt server:/directory`: copy file.txt to server:/directory
4. secure copy a directory to remote host: `scp -r [directory] [remotehost: path to where you want to save the directory]`