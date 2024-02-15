`sudo -l` displays what a user can run as sudo

`2>/dev/null`  treated as a blackhole, so you can put anything into this but you will not be able to get it back from

`find . -name file.txt 2>/dev/null` looks for _file.txt_ in current and sub-directories.

`find / -perm -u=s -type f 2>/dev/null` search for files that have SUID/GUID

  * **find** - Initiates the "find" command
  * **/** - Searches the whole file system
  * **-perm** - searches for files with specific permissions
  * **-u=s** - Any of the permission bits mode are set for the file. Symbolic modes are accepted in this form
  * **-type f** - Only search for files
  * **2>/dev/null** - Suppresses errors

