# cloud-dl

Please refer to the original GIT for acknowledgments!

Bash script to manage files on owncloud via webdav. cloud-dl allows you to list, upload, download, delete, move, create and share files.

**Added in this fork:**

* definition of the default sharing date limit on top of the code (7)
* mirror a local folder (structure and content, exclude hidden .files) (-m/--mirror)
* new function for sharing automatisation via CLI (-S/--share2)
* new function to get file & folder sizes in a share (-i/--info)
* new function to get file, folder sizes, and date last write in a share (-I/--info2)
* new dev function to get the full metadata content from the server (-z/--zap)

```
Usage: cloud-dl <options> [file|dir]
Options:
	 -l/--list [dir]                 List root directory or [dir]
	 -d/--download <file>            Download <file> to current location
	 -u/--upload <file> [dir]        Upload <file>. Optionally uploads <file> to [dir]
	 -m/--mirror <dir>               Mirror <dir> structure and content
	 -D/--delete <file|dir>          Delete file or directory
	 -k/--mkdir <dir>                Create new directory
	 -M/--move <source> <target>     Move file from remote <source> to remote <target> (e.g. --move file.txt somedir/file.txt)
	 -s/--share <file|dir> [-p] [-q] Create a public share and shows the url. Optionally -p prompts for a password, -q returns only the share URL
	 -S/--share2 <file|dir> <password> <days to share> 
	                                 Create a public share with password and returns '<url> | <password> | <sharing end date>‘
	 -U/--unshare <file|dir>         Delete a public share
	 -L/--list-shares                List shares
	 -i/--info [dir] [depth]         Get file size info for a share [dir] until [depth] (optional: default=1)
	 -I/--info2 [dir] [depth]        Get file size and date info for a share [dir] until [depth] (optional: default=1)
	 -z/--zap [dir] [depth]          Get raw content info for a share [dir] until [depth] (optional: default=1)
	 --configure                     Change connection configuration
	 -h/--help                       Show this help
# version: 1.7.2.1
```
