# Introduction
This DLL (Dynamic Link Library) app is an enhancement tool to be used to support [Glassconcpit FSX](https://play.google.com/store/apps/details?id=com.donotspeak.GlassCockpitFSX&hl=en). As a server application this DLL is used to transmit flight simulation data from FSX or P3D installed on host computers to android application ( [Glassconcpit FSX](https://play.google.com/store/apps/details?id=com.donotspeak.GlassCockpitFSX&hl=en) ).

# Requirement
- FSX / P3d game application on the host side computer.
- Simconnect SDK on the host computer, SDK version is depend on FSX and P3D version.
- [Glassconcpit FSX](https://play.google.com/store/apps/details?id=com.donotspeak.GlassCockpitFSX&hl=en) installed on android device.

# Installation
This application can be installed in the following way,
- Create `<AndroFSXServer>` folder in `<%USERPROFILE%>` directory.
![UserProfilePath](res/img/installation/UserProfilePath.png) 
- Extract, then place `<AndroFSXServer.cfg>` and `<AndroFSXServer.dll>` inside `<%USERPROFILE%\AndroFSXServer>` folder
![InstallTarget](res/img/installation/InstallTarget.png) 
- Add Add-ons, by modifying dll.xml
  - FSX USER dll.xml can be found in this path `<%USERPROFILE%\AppData\Roaming\Microsoft\FSX>`
  - PREPAD3D v2 dll.xml can be found in this path `<%USERPROFILE%\AppData\Roaming\Lockhead Martin\Prepar3D v2>`
- Update ip address in AndroFSXServer.cfg with your smarphone/tablet ip address (ipaddress of your phone can be found on setup page <slide down your current page>).
 
# Set up
After we're finish with installation step now we have to configure both client (android side) and server(host computer side).
1. On server side / host computer side. Update simulator dll.xml configuration file :
   1. **FSX USER** dll.xml configuration file can be found in this path `<%USERPROFILE%\AppData\Roaming\Microsoft\FSX>`
   1. **PREPAD3D v2** dll.xml configuration file can be found in this path `<%USERPROFILE%\AppData\Roaming\Lockhead Martin\Prepar3D v2>`
1. Update Host computer configuration.
   1. Find yours smartphone or tablet ip address. Can be found in setup page, slide left to open menu page.
   ![AndroidConfigStatus](res/img/set%20up/AndroidConfigStatus.jpg)
   1. Update AndroFSXServer.cfg, add smartphone or tablet ip address to AndroFSXServer.cfg 
   ![ConfigEdit](res/img/set%20up/ConfigEdit.png)
