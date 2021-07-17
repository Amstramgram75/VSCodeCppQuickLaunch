# VSCodeCppQuickLaunch
Quick Launch Visual Studio Code from Visual Studio Developer Command Prompt

## Why ?
When working on C++ project with Visual Studio Code, we have to start the IDE from the Visual Studio Developer Command Prompt.    
So, we fisrt need to launch Visual Studio Developer Command Prompt from the Windows Start Menu, then navigate to our working folder through some repetitive `cd` and finaly enter `code .` to  open Visual Studio Code.   
It bothers me !!!

## Take care !
Whatever the solution you choose, you must have added the Visual Studio Code *bin* folder in your path environment variable.  
Its path looks like this :   
`C:\Users\UserName\AppData\Local\Programs\Microsoft VS Code\bin`   
See [here](https://betanews.com/2015/11/23/windows-10-finally-adds-a-new-path-editor/) or [here](https://www.nextofwindows.com/three-alternative-windows-environment-path-editor) if you really don't know how to proceed.

## First Solution
I've written a *.inf* file that adds an entry to the context menu and allows automating the launch of Visual Studio Code in a given folder.

[![context Menu Entry Snapshot](https://github.com/Amstramgram75/VSCodeCppQuickLaunch/blob/main/Launch%20Visual%20Studio%20Code%20C++%20Here.png?raw=true)](#)

### Install
Just download the *LaunchVSCodeC++Here.inf* file, and install it through the **Install** entry in its context menu.

[![Install INF](https://github.com/Amstramgram75/VSCodeCppQuickLaunch/blob/main/Install%20INF.png?raw=true)](#)

### Uninstall
Go to the *Programs and Features*, find the *Launch Visual Studio Code C++ here for VS2019 Community* entry and double click to uninstall.

### Customization
You may adapt the different text labels as you like in the **[Strings]** section of the file.

**Be sure to set the right path for the VsDevCmd.bat file.   
The one specified in this file is for Visual Studio Community 2019 and may differ from the version you are using.**
