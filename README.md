# PoshCord-C2

**SYNOPSIS**

Using a Discord Server Chat and a github text file to Act as a Command and Control Platform.

**INFORMATION**

This script will wait until it notices a change in the contents of a text file hosted online (eg. github).
Every 10 seconds it will check a file for a change in the file contents and interpret it as a custom command. (updates can take upto 5 mins!)

**USAGE**

1. Setup the script
2. Run the script on a target.
3. Check discord for 'waiting to connect..' message.
4. Save the contents of your github file to contain 'options' to get a list of commands
5. Do the same with any other command listed - To run that module.

**MODULES**

= `Close`  : Close the Session                           =

= `Screenshot`  : Sends a screenshot of the desktop      =

= `Keycapture`   : Capture Keystrokes and send           =

= `Exfiltrate` : Send various files.                     =

= `Systeminfo` : Send System info as text file.          =

= `TakePicture` : Send a webcam picture.                 =

= `FolderTree` : Save folder trees to file and send.     =

= `FakeUpdate` : Spoof windows update screen.            =

= `CustomCommand` : Execute a github file as a script.   =

**SETUP**

1. change YOUR_GITHUB_FILE_URL to the url for the file that contains the command eg. https://raw.githubusercontent.com/Username/Repo/main/file.txt
2. change YOUR_WEBHOOK_URL to your webhook eg. https://discord.com/api/webhooks/123445623531/f4fw3f4r46r44343t5gxxxxxx

**EXTRA**

You can add custom scripting in a secondary github file, change YOUR_OTHER_GITHUB_FILE_URL to another text file and add code to it,
then in the first github file save it with 'customcommand' as the contents 

Killswitch : save github file contents as 'kill' to stop 'KeyCapture' or 'Exfiltrate' command and return to waiting for commands.
