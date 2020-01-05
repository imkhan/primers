Getting Help

[command] --help
[command] -h
[command] help
man [command]

whoami
w
uname -a 
uname


ls -alh   [h flag is for human friendly file size]

cat file_xyz.txt | more
cat file_xyz.txt | wc -w.  [word count]
cat file_xyz.txt | grep searchword | wc -w

tree > tree.txt (Replaces the file content)
tree >> tree.txt (Appends to file content)
more < data.txt 

Archiving And Compression

gzip big_file.txt      (deletes original file, and creates big_file.txt.gz)
gzip -d big_file.txt.gz (decompresses the gzip file to original file)

Better alternative is 'tar'

tar -cvzf foldername.tgz foldername (flags: create, verbose, gzip, filename)
tar -xvzf foldername.tgz (extracts a tar file)


rm -i file  (remove with confirmation)
rm -r dir   (remove recursively all directories and contents under 'dir')
rm -f dir   (force removal without confirmation)


mv or cp (-n: don't overwrite, -v: be verbose, -i: interactive, -f: force, ignore -i and -n)


mkdir -p dir1/dir2/dir3   (-p: creates nested directories)
rmdir foldername    (removes empty directory as well)

Permissions

-rwxrwxrwx :: [directory][user][group][other]

Read:4
Write:2
Execute:1

Change Mode
chmod u+w file    (gives write permission to user)
chmod g-rw file   (removes read and write permissions from the group)
chmod u=rwx,go=r file (gives all permissions to user and read permission to group and other)
chmod a+r fike    (gives read permission to all: user, group, and other)

Change Group

chgrp everyone

Change Owner

chown root file (only root user allowed: so use sudo)

Check SCP andd SFTP commands for file transfers to remote machines



echo $PATH    (Show path to bin directory)



^a   Goto begining of a line
^e   Goto end of a line
^k   Delete words on the right
^w   Delete a word from left
ESC-b Move cursor one word back
ESC-f Move cursor one word forward



top -o cpu (ordered by CPU)
top -o vsize (ordered by memory)


~/.zshrc ----> source ~/bin/dotfiles/[bash/zsh]/aliases

Check
