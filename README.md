#OSVR_Quick_Start
Author: BinZ@SUSTech  
[Look at My Github](https://github.com/ideaRunner/OSVR-Start)
##Please Note
This is a step-by-step tutorial that how to quickly start OSVR HDK2.  
My graphic card is GTX1060, driver version is 376.xx and operating system is Windows10.  
This article also can help those persons who use high Nvidia GPU driver version.  
The official getting start tutorial you can find [Here](https://github.com/OSVR/OSVR-Docs). There is a official instruction of [Nvidia GPU driver](https://github.com/OSVR/OSVR-Docs/blob/master/Troubleshooting/RenderManager.md#compatible-gpu-drivers) 

#Software Preparation
There is the official [download page](http://osvr.github.io/using/). If you want to save time and do not download from official page, you can download at [my Github](https://github.com/ideaRunner/OSVR-Start).

1. **OSVR Runtime for Windows**  
   * Official [download page](http://osvr.github.io/using/).
   * OSVR Runtime installer includes everything you need to get OSVR up and running (not for development, but everything for running)  
	![Runtime](https://github.com/ideaRunner/Images/raw/master/OSVR/Software%20Preparation/Runtime.png)
   * Click [**Download**](http://access.osvr.com/binary/osvr-runtime-installer) to enter the download page.  
   ![Runtime2](https://github.com/ideaRunner/Images/raw/master/OSVR/Software%20Preparation/Runtime2.png)
   * Choose the newest core version that is listed first. Make sure the software bits are matching your system. 
   * Click and then begin to download OSVR Runtime.  
2. **No need to Download OSVR SDK for Windows**  
   * If you only want to run OSVR HDK2 to play some demos or games, **No** need to download *OSVR SDK*, Otherwise you can click and download at [this page](http://osvr.github.io/using/).
3. **OSVR HDK Windows Driver Pack**  
   * These are drivers for OSVR HDK2.
   * Click [**Download**](https://github.com/OSVR/OSVR-HDK-Windows-Drivers/releases) to enter the download page.  
   ![Driver](https://github.com/ideaRunner/Images/raw/master/OSVR/Software%20Preparation/Combined-driver.png)
   * If you want to run or play first, you can select the newest version of combined driver (exe file). Example: *OSVR-HDK-Combined-Driver-Installer-1.2.8.exe* 
   * No need to download other files such as *Source Code* or *inf file*.
4. **SteamVR-OSVR**  
   * Before you use SteamVR-OSVR, **Steam** and **SteamVR** must be installed in your PC. You can search it on Google.  
   * SteamVR-OSVR is a very useful tool to use OSVR HDK2. Without it we may have some problems with Direct Mode and Extended Mode because of our higher GPU driver version.
   * [Official page](https://github.com/OSVR/SteamVR-OSVR) and [Download page](https://bintray.com/osvr/SteamVR-OSVR/SteamVR-OSVR-Win/v0.1-296-g7011d81-core-v0.6-1935-ga2cba4b6#files)
   * You can download it at **Files** bar. It is a *7z* Compressed file.  
   ![SteamVR](https://github.com/ideaRunner/Images/raw/master/OSVR/Software%20Preparation/SteamVR.png)
   
#Software Installation

1. **Install OSVR Runtime**
	* Open OSVR Runtime installer. Exmaple:OSVR-Runtime-vxx.msi
	* Recommend you to install by default.
2. **Install OSVR HDK Windows Driver Pack**  
	* Before you install the Combined-Driver, make sure all your OSVR devices unconnect your PC.
	* Open driver installer.
	* It will not cost much time.
3. **SteamVR-OSVR**  
	* Make sure you have installed Steam and SteamVR. If have not, you can search it on google, it is very simple.
	* Unzip the SteamVR-OSVR file. Example: SteamVR-OSVR-Win-Build-v0.1-296-g7011d81-core-v0.6-1935-ga2cba4b6.7z
	* Open the folder you created.  
	![SteamVR](https://github.com/ideaRunner/Images/raw/master/OSVR/Install/SteamVR1.png)
	* Open ...\SteamVR-OSVR\lib\openvr  
	![SteamVR](https://github.com/ideaRunner/Images/raw/master/OSVR/Install/steamVR2.png)
	* You will see a folder named **osvr**. **Copy** it.
	* Find your steam folder in your PC. 
	* Open ...\Steam\steamapps\common\SteamVR\drivers  
	![SteamVR](https://github.com/ideaRunner/Images/raw/master/OSVR/Install/steamVR3.png)
	* You may see some other VR devices driver. **Paste** it.
	* Finish.  

#How to Start
Please notice that 1. Preparation and 2. Configuration only need to be done **once**.
   
1. **Preparation**  
    * Follow your instructions to connect the lines of OSVR HDK2.
    * Power it.
    * Open **OSVR Central** which is included in OSVR Runtime. You can find it in your windows start menu.  
    ![Central](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR%20Central1.png)

2. **Configuration**
    * Please check your configuration if this is the first time you use HDK2 or you have not checked it yet.
    * Click **Tools** in the menu bar.
    * Click **OSVR Configurator**.  
    ![Conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator.png)
    * Then it will open your browser: http://localhost:5000/#/  
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator2.png)
    * Click **Devices** at Menu bar.  
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator3.png)
    * Choose **OSVR_HDK_2_0.json**, Click Use.
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator4.png)
    * Click **Rendering** at Menu bar.   
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator5.png)
    * In **Direct Mode**, Click **Disable**.  
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator6.png)
    * In **Samples**, find osvr_server_config.HDK20**Extended**Landscape.sample.json, click **Use**.  
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator7.png)
    * Close OSVR Configurator and back to **OSVR Central** which we have opened in windows start menu.
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Configurator8.png)
    * Click **Enable Extended Mode**.
    * Configuration is finished, you can start OSVR Server. Configuration only need to be done once.

3. **Start OSVR Server**
    * Click **Tools** in the menu bar.
    * Click **Start OSVR Server**. Remember that every time the first thing to use OSVR is **Start OSVR Server**.
    ![conf](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/OSVR_Server1.png)
    * Then you will see a black Dos Shell.
    * Hold your head/HMD closer than 0.3 meters from the tracking camera for a few minutes. You can watch the instruction in the Shell.

4. **Start SteamVR**  
    * Open your Steam, Select **TOOLS** in the **LIBRARY** bar.   
    ![SteamVR](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/SteamVR.png)  
    * Open your SteamVR.   
    ![SteamVR](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/SteamVR2.png)
    * If you can see the two green devices in SteamVR bar, it means your Combined-drivers of HDK2 has been installed successfully as well as your SteamVR-OSVR driver you copied early. If not, check your drivers.  
    ![SteamVR](https://github.com/ideaRunner/Images/raw/master/OSVR/Start/SteamVR3.png)
    * If you see the green **Ready** in SteamVR bar,awesome,you finish. You can use SteamVR do anything you want.
    * If you see the red **Not Ready**, do not lose heart. You are very close to your success. See the **Quick Trouble Shooting**.

5. **Watch VR videos or Play Games with SteamVR**  
    * You need to **Run Room Setup** under SteamVR instructions 
    * Then you can download or pruchase some applications in the Steam STORE.
    * For VR video, I suggest *Simple VR Video Player*. It has a good user experience in playing VR videos.  
    * After that, You can do anything you want.

###SteamVR Warning
If your SteamVR is green **Ready**. Please do not apply the suggestions that SteamVR recommended. Because the suggestions may cause some problems.   
You can have a try if you want, and the worst thing is to recopy the SteamVR-OSVR files.

#Quick Trouble Shooting
1. **SteamVR Not Ready: Compositor is not fullscreen**: 
	* Close all the VR applications in SteamVR.
	* Click **Make Compositor fullscreen**, if nothing happens, launch some other VR applications or restart SteamVR.
	* It happens because VR apps have default settings of SteamVR. some of them may not supplied by OSVR.
	* If useless, recopy SteamVR-OSVR files is our last way.
2. **SteamVR Not Ready: Headset not deteced**: 
    * Make sure you have start OSVR Server before.
    * Check your headset connection.
    * **Restart** SteamVR.
3. **Extended Mode: One lens light, the other lens off**:
	* It is hardware part of the line connection problem.
	* Reconnect the 
4. **Extended Mode: Some applications are open on our lenses**:
	* There are hotkeys can help you move those applications in your main screen.
	* Open those applications.
	* Press **Win + ←** or **Win + →** serveral times.
	* The applications will move between your screen and lenses.  
5. **Extended Mode: Something wrong**
	* If somethings wrong and you can not change the screen setting by using your mouse.
	* Press **Win + P** slowly serveral times untill it back to normal.
	* **Win + P** is the the hotkey to change the setting of multiple screens.  
	


##Reference video
[Setting Up SteamVR on a OSVR HDK2 [Nvidia]](https://www.youtube.com/watch?v=TCA0CBXmS2Q&feature=youtu.be)  
[Setting up SteamVR on a OSVR HDK2 [Radeon]](https://www.youtube.com/watch?v=9Uju31UYWBM)








