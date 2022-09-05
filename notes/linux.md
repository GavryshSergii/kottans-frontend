

- ls - list the contents of a directory (look at structure);
- ls -l - list content with long listing option (type - first symbol, security, owner, groupe, size, last_mod, name);
# security
- user (owner)   --- or rwx;
- group;
- other (world);
- The 'r' means you can "read" the file's contents.
- The 'w' means you can "write", or modify, the file's contents.
- The 'x' means you can "execute" the file.
- chmod - change mode
  $ chmod [references][operator][modes] file
# references
- u - user
- g - group
- o - others
- a - all
# operator
- + - adds the specified modes
- - - removes the specified modes
- = - the modes specified are to be made the exact modes
# modes
- r - read
- w - write
- x - execute


- cd directory - change directory;
- pwd - print working directory;
- ~ - in path refer to home directories
    cp ~/jokes /tmp
- ~IDUser - in path refer to User home directories
    cp ~bookie/jokes /tmp - cp /home/bookie/jokes /
- df - report file system disk space usage 
- df directory - report file system disk space usage 
- ps aux - report a snapshot of the current processes. (aux - To see every process on the system using BSD syntax)
- ps aux | grep keyword - filter the results of the first command by keyword
- kill PID - send a signal to a process;
- kill -9 PID - 

- more file - display content file, press spacebar to see next page;
- mkdir name_new_directory - make directory;
- mv file directory - move file into directory;
- mv file new_file_name - rename file or directory;
- cp file_name new_file_name - copy file;
- cp -r directory directory_to_copy_to - copy directories


- rm file_name - remove file;
- rmdir directory_name - remove directory;

- man - help command
  man chmod - help chmod command
- man -k keyword 
    man -k user - search on the word "user"
- find - search for files in a directory hierarchy
    find ~ -name "poem*"
- cat file_1 file_22 ... - displays the content of several files
- cat file_1 file_2 > new_file - > create/over-write in new_file
- cat file_1 file_2 >> old_file - >> keep the previous contents of old_file and simply append to it

- lpr - send to printer
  lpr file_name
  lpr -P printer_name file_name - send your file to a printer called "printer_name"


- lpq - display print queue
  lpq -P printer_name
- lprm -remove from print queue
  lprm -P printer_name job_number





cat	concatenate (combine) two or more files
cd	change to another directory
chmod	change mode (security permissions) of file or directory
ugo+-rwx	user (owner), group, other (world), add, remove, read, write, execute
cp	copy file
-r	copy directory tree
df	show disk free information
find	find files in a directory tree
finger	display user information
grep	list text lines containing particular characters
groups	show your security group memberships
kill	kill process
-9	kill process immediately
lpr	send to printer
-P	send to another printer
lpq	show status of print queue
-P	show print jobs in a different print queue
lprm	remove print job from printer
-P	remove from a different print queue
ls	list contents of current directory
-l	long (detailed) listing
man	display portion of online Unix manual
-k	display command descriptions relating to subject keyword
mkdir	make new directory
more	display contents of file
mv	move or rename file or directory
ps aux	list status of all processes (running programs)
pwd	print working (current) directory
rm	remove file
-r	remove directory tree
rmdir	remove an empty directory
..	parent directory
.	current directory
*	wildcard representing any combination of characters
?	wildcard representing exactly one character
~	your home directory
~userid	userid's home directory
> 	send output to file
>> 	append (add) output to file
|	pipe output from one command as input to another
