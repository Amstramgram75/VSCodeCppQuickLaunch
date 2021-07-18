# VSCodeCppQuickLaunch
Two easy ways to quick Launch Visual Studio Code from Visual Studio Developer Command Prompt.

## Why ?
When working on C++ project with Visual Studio Code, we have to start the IDE from the Visual Studio Developer Command Prompt.    
So, we first need to launch Visual Studio Developer Command Prompt from the Windows Start Menu, then navigate to our working directory through some repetitive `cd` and finally enter `code .` to  open Visual Studio Code.   
I don't know about you but it bothers me !!! :unamused:

## Take care !
:stop_sign:
**Whatever the solution you choose, you must have added the Visual Studio Code *bin* folder in your path environment variable.**
:stop_sign:

Its path looks like this :   
`C:\Users\UserName\AppData\Local\Programs\Microsoft VS Code\bin`   
See [here](https://betanews.com/2015/11/23/windows-10-finally-adds-a-new-path-editor/) or [here](https://www.nextofwindows.com/three-alternative-windows-environment-path-editor) if you really don't know how to proceed.
___
___

## First Solution
>Credit goes to [Daniel Cazzulino aka KZU](https://github.com/kzu/CommandPromptHere).  

Just an *.inf* file that adds an entry to the context menu and allows automating the launch of Visual Studio Code in a given folder.

[![context Menu Entry Snapshot](https://github.com/Amstramgram75/VSCodeCppQuickLaunch/blob/main/img/Launch%20Visual%20Studio%20Code%20C%2B%2B%20Here.png?raw=true)](#)

### Install
Download the *LaunchVSCodeC++Here.inf* file and install it through the **Install** entry in its context menu.

[![Install INF](https://github.com/Amstramgram75/VSCodeCppQuickLaunch/blob/main/img/Install%20INF.png?raw=true)](#)

### Uninstall
Go to *Programs and Features*, find the *Launch Visual Studio Code C++ here for VS2019 Community* entry and double click to uninstall.

### Customization
You may adapt the different text labels as you like in the **[Strings]** section of the file.

:stop_sign: **Be sure to set the right path for the VsDevCmd.bat file.   
The one specified in this file is for Visual Studio Community 2019 and may differ from the version you are using.** :stop_sign:
___
___

## Second solution
A basic batch calling Visual Studio *VsDevCmd.bat* and then `code .`.  
:stop_sign: **As previously, you have to set the right path for the VsDevCmd.bat file.** :stop_sign:   
That's done, just copy *LaunchVSCodeC++Here.bat* in your working directory and launch it...
