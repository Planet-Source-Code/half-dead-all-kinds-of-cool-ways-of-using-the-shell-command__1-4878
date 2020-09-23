<div align="center">

## all kinds of cool ways of using the shell command


</div>

### Description

These different ways of using the shell command will let you : Launch files without knowing the associated program(doc,bmp,zip,etc), copy files and complete directories, run dos commands, launch a browser, launch an email client with almost all fields prefilled(including body!) and loads of stuff you might think of.
 
### More Info
 
You dont get any feedback from VB to check if the operation went well, so use this only for stuff that you are sure about, and dont need error codes returned.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Half\-Dead](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/half-dead.md)
**Level**          |Beginner
**User Rating**    |4.1 (74 globes from 18 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Files/ File Controls/ Input/ Output](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/files-file-controls-input-output__1-3.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/half-dead-all-kinds-of-cool-ways-of-using-the-shell-command__1-4878/archive/master.zip)





### Source Code

```
'The vbhide makes sure that ppl dont see that ugly dosbox
Shell ("c:\windows\command\xcopy /e /i /r c:\temp d:\NewTemp"), vbHide
' will create a directory called NewTemp on d: and copy
' all the files and directories recursively from c:\temp
' into it, without showing the dosbox
' you can also run any commands like del, dir, etc
' by running command.com
shell("command.com /c PathandFileToRun Commuters CommandLine"), vbHide
' /c tells command.com to run a command and exit
' you could run somethin like :
Shell ("command.com /c dir /b d:\ > dListing.txt"), vbHide
' and recover all the names of the files in d:
' or run files associated to programs(doc,zip,bmp,etc)
' by using the start command, windows will launch the
' file with the appropriate program
Shell ("start C:\WINDOWS\HELP\WINHLP32.HLP"), vbHide
' if you need even more dos power then you could just as easily run
' some bat files to do bigger operations. I think
' windows scripting host can do some awesome stuff too
' but im not familiar with it at all. All i know is
' that it lets you write javascript and vbscript like
' batch files.
Shell ("start http://www.whatever.com"), vbHide
'Will launch the default webrowser on that page
Shell ("start mailto:me@test.com,next@next.com?cc=whoever@whetever.com&subject=whatever&body=your text"), vbHide
'launch the default email client with most fields prefilled.
'im sure you can attach a file, but i havent found the right
'command yet. also its VERY important the order in which the
'commands are fed. Just separate multiple adresses with a comma
'like above.
'if i find any other cool usages i'll postem up.
```

