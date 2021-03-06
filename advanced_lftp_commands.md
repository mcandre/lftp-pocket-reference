# Advanced LFTP Commands

Graphical FTP clients tend to offer a side-by-side view of local vs. remote files. LFTP presents all this information in one view, using distinct commands for referring to local vs. remote files.

## Remote operations

LFTP assumes most operations run remotely by default, using Unix-style commands for directory navigation, file copying, and moving. E.g., `pwd` in an LFTP session prints the current working directory of the remote FTP endpoint. The same goes for `cd`, `ls`, `mkdir`, `mv`, `cp`, `rm`, and other common Unix file commands.

## Local operations

To navigate directories and perform other local operations, prefix the operation with `local `. E.g., `local pwd` prints the current working directory of the local FTP endpoint. The same goes for `local cd`, `local ls`, `local mkdir`, `local mv`, `local cp`, `local rm`, `local move`, `local copy`, `local rm`, `local rmdir`, and other common shell commands.