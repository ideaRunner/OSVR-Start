#OSVR_Quick_Start
##Please Note

This is a step-by-step tutorial that how to quickly start OSVR HDK2.  
My graphic card is GTX1060, deriver version is 376.xx and operating system is Windows10.  
This article also can help those persons who use high Nvidia GPU driver version.  
The official getting start tutorial you can find [Here](https://github.com/OSVR/OSVR-Docs). There is a official instruction of [Nvidia GPU driver](https://github.com/OSVR/OSVR-Docs/blob/master/Troubleshooting/RenderManager.md#compatible-gpu-drivers) 

#Software Preparation
There is the official [download page](http://osvr.github.io/using/). If you want to save time and do not download from official page, you can download at my [Github](https://github.com/ideaRunner/OSVR-Start).

1. **OSVR Runtime for Windows**  
   * OSVR Runtime installer includes everything you need to get OSVR up and running (not for development, but everything for running)  
   * Click [**Download**](http://access.osvr.com/binary/osvr-runtime-installer) to enter the download page.
   * Choose the newest core version that is listed first. Make sure the software bits are matching your system. 
   * Click and then begin to download OSVR Runtime.  
2. **No need to Download OSVR SDK for Windows**  
   * If you only want to run OSVR HDK2 to play some demos or games, **No** need to download *OSVR SDK*, Otherwise you can click and download at [this page](http://osvr.github.io/using/).
3. **OSVR HDK Windows Driver Pack**  
   * These are drivers for OSVR HDK2.
   * Click [**Download**](https://github.com/OSVR/OSVR-HDK-Windows-Drivers/releases) to enter the download page.
   * If you want to run or play first, you can select the newest version of combined driver (exe file). Example: *OSVR-HDK-Combined-Driver-Installer-1.2.8.exe* 
   * No need to download other files such as *Source Code* or *inf file*.
4. **SteamVR-OSVR**  
   * Before you use SteamVR-OSVR, **Steam** and **SteamVR** must be installed in your PC. You can search it on Google.  
   * SteamVR-OSVR is a very useful tool to use OSVR HDK2. Without it we may have some problems with direct mode and extend mode because of our higher GPU driver version.
   * [Official page](https://github.com/OSVR/SteamVR-OSVR) and [Download page](https://bintray.com/osvr/SteamVR-OSVR/SteamVR-OSVR-Win/v0.1-296-g7011d81-core-v0.6-1935-ga2cba4b6#files)
   * You can download it at **Files** bar. It is a *7z* Compressed file.
   
#Software Installation

1. **Install OSVR Runtime**
	* Open OSVR Runtime installer. Exmaple:OSVR-Runtime-vxx.msi
	* Recommend you to install by default.
2. **Install OSVR HDK Windows Driver Pack**  
	* Before you install the Combined-Driver, make sure all your OSVR devices unconnect your PC.
	* Open driver installer.
	* It cost little time.
3. **SteamVR-OSVR**  
	* Make sure you have installed Steam and SteamVR. If have not, you can search it on google, it is very simple.
	* Unzip the SteamVR-OSVR file. Example: SteamVR-OSVR-Win-Build-v0.1-296-g7011d81-core-v0.6-1935-ga2cba4b6.7z
	* Open the folder you created.
	* Open ...\SteamVR-OSVR\lib\openvr
	* You will see a folder named **osvr**. **Copy** it.
	* Find your steam folder in your PC. 
	* Open ...\Steam\steamapps\SteamVR\drivers
	* You may see some other VR devices driver. **Paste** it.
	* Finish.  

#How to Use
####Preparation
1. Follow your instructions to connect the wires of OSVR HDK2.
2. Power it.
3. Open **OSVR Central** which is included in OSVR Runtime. You can find it in your windows start menu.

####Configuration
1. Please check your configuration if this is the first time you use HDK2 or you have not checked it yet.
2. Click **Tools** in the menu bar.
3. Click **OSVR Configuration**.

#####Start
4. Click **Tools** in the menu bar.
5. Click **Start OSVR Server**. Remember that every time the first thing to use OSVR is **Start OSVR Server**.
6. Then you will see a black Dos Shell.
7. Hold your head/HMD closer than 0.3 meters from the tracking camera for a few minutes. You can watch the instruction in the Shell.
8. Open your Steam, Select **TOOLS** in the **LIBRARY** bar.
9. Open your SteamVR. 
10. If you can see the two green devices in SteamVR bar, it means your Combined-drivers of HDK2 has been installed successfully as well as your SteamVR-OSVR driver you copied early. If not, check your drivers.
11. If you see the green **Ready** in SteamVR bar,awesome,you finish. You can use SteamVR do anything you want.
12. If you see the red **Not Ready**, do not lose heart. You are very close to your success. See the **Quick Trouble Shooting**.

#Quick Trouble Shooting
###SteamVR Warning
If your SteamVR is green **Ready**. Please do not apply the suggestions that SteamVR recommended. Because the suggestions may cause some problems.   
You can have a try if you want, and the worst thing is to recopy the SteamVR-OSVR files.

1. **SteamVR Not Ready: Compositor is not fullscreen**: 
	* Close all the VR applications in SteamVR.
	* Click **Make Compositor fullscreen**, if nothing happens, launch some other VR applications or restart SteamVR.
	* It happens because VR apps have default settings of SteamVR. some of them may not supplied by OSVR.
	* If useless, recopy SteamVR-OSVR files is our last way.
2. **Extend Mode: One lens light, the other lens off**:
	* It is hardware part of the line connection problem.
	* Reconnect the 
3. ****


##Reference video
[1](https://www.youtube.com/watch?v=TCA0CBXmS2Q&feature=youtu.be)
[2](https://www.youtube.com/watch?v=9Uju31UYWBM)








