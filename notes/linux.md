

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
  

