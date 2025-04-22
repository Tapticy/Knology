
`cd (Change Directory)` 
Usage: cd DIRECTORY-NAME Example: cd C:\Users\YourName – Moves to your account folder. Special Cases: cd .. – Moves one level up in the directory tree. cd \ – Takes you to the root directory of the current drive^2^.

`dir (Directory)`
Usage: dir Example: dir /P – Lists the contents of the current directory, pausing after each screen-ful. Special Cases: /A:H – Lists all hidden files in the current directory^2^.

`mkdir (Make Directory)` 
Usage: mkdir DIRECTORY-NAME Example: mkdir "My_Files" – Creates a new folder named "My Files" in the current directory^2^.

`rmdir (Remove Directory)` 
Usage: rmdir DIRECTORY-NAME Example: rmdir "My_Files" – Deletes the folder named "My_Files" if it is empty^2^.

`copy` 
Usage: copy SOURCE/PATH DESTINATION/PATH Example: copy file1.txt C:\Backup – Copies a file named "file1.txt" to the "Backup" folder^2^.

`del (Delete)` 
Usage: del FILENAME Example: del file1.txt – Deletes the file named "file1.txt" from the current directory^2^.

`ren (Rename)` 
Usage: ren OLD_FILENAME NEW_FILENAME Example: ren old_file.txt new_file.txt – Renames the file "old_file.txt" to "new_file.txt"^2^.

`cls (Clear Screen)` 
Usage: cls – Clears the screen contents^2^.

`ipconfig (Internet Protocol Configuration)` 
Usage: ipconfig Example: ipconfig /all – Displays detailed network information^2^.

`ping` 
Usage: ping DNSNAME-OR-IP Example: ping google.com – Checks network connectivity to Google's servers^2^.

`tracert (Trace Route)` 
Usage: tracert DOMAIN-NAME Example: tracert google.com – Traces the route to Google's servers^2^.

`shutdown` 
Usage: shutdown /s – Shuts down the computer immediately. Example: shutdown /r /t 30 – Restarts the computer after a 30-second delay^2^.

tasklist Usage: tasklist Example: tasklist /V – Shows detailed information about running processes^2^.

taskkill Usage: taskkill /IM PROCESS-NAME Example: taskkill /IM notepad.exe – Ends the Notepad process^2^.

`chkdsk` or `chkdsk C: /f /r /x `  
Usage: chkdsk /f Example: chkdsk C: /f – Checks the "C:" drive for errors and attempts to fix them. After restart.

Method 2: Using DISM tool commands in CMD
Before repairing Windows using the DISM tool, we will check the health and integrity of the Windows component store.

Type the following commands: DISM /Online /Cleanup-image /Checkhealth


sfc /scannow (System File Checker) Usage: sfc /scannow – Scans and repairs corrupted system files.

help Usage: help COMMAND-NAME Example: help dir – Shows information about the "dir" command^2^.

exit Usage: exit – Closes the current command window^2^.

winget (Windows Package Manager) Usage: winget install APP-NAME Example: winget install "Mozilla Firefox" – Installs the Mozilla Firefox browser^2^.

sudo (Superuser Do) Usage: sudo COMMAND Example: sudo del file.txt – Runs the delete command as an administrator^2^.


