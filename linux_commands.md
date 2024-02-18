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


Copy a Remote File to a Local System using the scp Command: `scp remote_username@remote_ip:/remote/file.txt /local/directory`. For more info [SCP Commands](https://linuxize.com/post/how-to-use-scp-command-to-securely-transfer-files/#:~:text=Unlike%20rsync%2C%20when%20using%20scp%2C%20you%20don%E2%80%99t%20have,on%20the%20remote%20host%20host2.com.%20scp%20user1%40host1.com%3A%2Ffiles%2Ffile.txt%20user2%40host2.com%3A%2Ffiles)

---

**Helpful Links**

[GTFOBins](https://gtfobins.github.io/)

[OSCP Guide](https://sushant747.gitbooks.io/total-oscp-guide/content/)

[Linux - Privelege Escalation](https://swisskyrepo.github.io/InternalAllTheThings/redteam/escalation/linux-privilege-escalation/#tools)
