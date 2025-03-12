# FAQ - Troubleshooting

* Q: **What if my levels won’t launch on the Render PCs?**  
  * 1\) Open project on Render1 to make sure there is a plugin missing (e.g. Cargo).  
    * Disable Cargo in main project, resync files, launch  
  * If still wont launch (“CLOSED”) on Render PCs)...  
    * Try the Mikey Method…  
* Q: **HDRI Backdrop is fighting with Skylight (ambient light goes off)**  
  * Seems to be a bug in UE5.3  
  * Try Save Current Level As…  
* Q: In a low-light/”overcast” scene, **my background (e.g. grass) is “shimmering”**  
  * (Looks like noise or static)  
  * Freeze the screen (if possible)  
  * ChatGPT suggestions: [link](https://chatgpt.com/share/67bdf442-879c-8010-9777-c30230e40ab0) (Lumen, lighting)  
* Q: **Level Sequence not updating** on the wall  
  * A: Try clicking the “save” icon inside the Level Sequence UI (top bar)  
* Graphic of the VP components we need to learn:  
  * Unreal 5.3  
  * Switchboard  
  * Multi-user editing  
  * File syncing  
  * Perforce  
* Make lights static so they can bake  
  * vs stationary?  
* My project launches on the Render PCs but not on my Control PC  
  * Might be another instance of Unreal running on the Control PC. Check Task Manager and End Task for Unreal. Or: shut down switchboard and reboot the control PC  
* My project launches on Control PC but not the render PCs  
  * Might be a missing plugin. Switch to the Render PC and see if an alert is displayed (eg Cargo). If it is, dismiss it (“proceed without installing the plugin”)  
