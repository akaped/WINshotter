# WINshotter
## Powershell script that allows to take recurrent screenshots from a Windows machine and send it to a remote FTP server. 


This is my first try with __Windows Powershell__. I needed to being able to monitor the activity of a remote windows machine without any other user intervention. I couldn't find a similar software online so I've created my customised implementation. 

The usage is really sample. 

1. Download the zip or git clone this repository. 
2. Edit WINshotter.ps1 
- Change the FTP server address
- Change Username and PSW
- Eventually change where the temporary screenshot is saved.
- Activate/Deactivate the hide function. 
3. Run WINshotter.ps1 through Windows Powershell. 


! You obviously need to have a FTP server up and running !
PAY ATTENTION. THis script DOES NOT USE an encrypted protocol to transfer the data, this means that a MITM attack will spoof easily your USR and PSW or the content you are transferring to the server. 
Soon I will release a new implementation that includes the option to use FTPS. 

I needed this script to run when windows booted and the user logged in. So I've packed it into an exe with PS2EXE and added the activity to the Windows Tasker utility. 

Contact me if you need more info. 
