# cloud-dl

Please refer to the original GIT for acknowledgments!

Bash script to manage files on owncloud via webdav. cloud-dl allows you to list, upload, download, delete, move, create and share files.

**Added in this fork:**

* definition of the sharing date limit
* new function for sharing automatisation via CLI (-S/--share2)
* new function to get file & folder sizes in a share

```
Usage: cloud-dl <options> [file|dir]
Options:
   -l/--list [dir]                 List root directory or [dir]
   -d/--download <file>            Download <file> to current location
   -u/--upload <file> [dir]        Upload <file>. Optionally uploads <file> to [dir]
   -D/--delete <file|dir>          Delete file or directory
   -k/--mkdir <dir>                Create new directory
   -M/--move <source> <target>     Move file from remote <source> to remote <target> (e.g. --move file.txt somedir/file.txt)
   -s/--share <file|dir> [-p] [-q] Create a public share and shows the url. Optionally -p prompts for a password, -q returns only the share URL
   -S/--share2 <file|dir> <password> <days to share> Create a public share with password and returns the url, password, and <sharing end date>
   -L/--list-shares                List shares
   -i/--info [dir]                 Get file size info for a share [dir]
   -U/--unshare <file|dir>         Delete a public share
   --configure                     Change connection configuration
   -h/--help                       Show this help
```
