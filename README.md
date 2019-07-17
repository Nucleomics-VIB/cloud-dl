# cloud-dl

Bash script to manage files on owncloud via webdav. cloud-dl allows you to list, upload, download, delete, move, create and share files.

With new functions for automatisation

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
   -S/--share2 <file|dir> <password> Create a public share with password and returns the url and password (@SP)
   -L/--list-shares                List shares
   -U/--unshare <file|dir>         Delete a public share
   --configure                     Change connection configuration
   -h/--help                       Show this help
```
