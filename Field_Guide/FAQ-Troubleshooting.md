# FAQ - Troubleshooting



**Q: My project launches on Control PC but not the render PCs**

  * Might be a missing plugin: Switch to the Render PC and see if an alert is displayed (eg Cargo). If it is, dismiss it (proceed and disable the plugin) and it should remember that state and run without incident thereafter.  Uninstall that plugin from your Control PC next time.
  * If not, try the "Mikey Method": 
    * TBD: describe adding level instance into NDC level



**Q: My project launches on the Render PCs but not on my Control PC**  

  * Might be another instance of Unreal running on the Control PC. Check Task Manager and End Task for Unreal. Or: shut down switchboard and reboot the control PC  



**Q: Level Sequence not updating on the wall (e.g. play, object edit)**  

  * A: Try clicking the “save” icon inside the Level Sequence UI (top bar)  



**Q: HDRI Backdrop is fighting with Skylight (ambient light goes off)**  

* IF using an HDRI backdrop, you may see the ambient light switch off suddenly.  This seems to be a bug in UE5.3.  Try "Save Current Level As…" and save the current level with the same name in the same Content Drawer location -- this sometimes clears up the problem!



**Q: In a low-light/”overcast” scene, my background (e.g. grass) is “shimmering”** 

  * Freeze the LED Volume screen (if possible)  
  * Other suggestions: [link](https://chatgpt.com/share/67bdf442-879c-8010-9777-c30230e40ab0) (Lumen, lighting)  

