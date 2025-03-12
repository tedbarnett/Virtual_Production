# Performance Optimization

* What is your average framerate?  
  * To see your FPS:  
    * Enable menu bar FPS view: Edit/Editor Preferences/”Show Frame Rate and Memory” \- check the box  
    * Can also enter “stat unit” and “stat fps” in CMD box at bottom of window (or press “‘“ key to open) to show on screen overlay  
  * Note: Stat Unit shows 2 key values:  
    * **Game**: time running on CPU  
    * **GPU time**: time running on GPU  
      * If GPU value is higher, then it is the main bottleneck (it usually is\!)  
* **Lighting**  
  * Check: Light Complexity  
    * Click “Lit” bubble at top of editor viewport, select “Optimization Viewmodes → Light Complexity”  
    * Look for problem areas (white or red areas) with too many overlapping lights  
  * Solutions:  
    * Try disabling lights: delete ones that don’t matter  
    * Reduce attenuation radius for lights  
    * Disable Directional Light if indoors and not seen  
    * Other?  
* **Lumen**  
  * Try disabling Lumen to see if it helps  
  * 3 places to look for it:  
    * 1\) Project Settings/Dynamic Global Illumination: set to “Screen Space (Beta)” to disable Lumen default  
    * 2\) Any Post Process Volume in the level itself  
      * Note: Might want to delete this and rely on the Post process volume already inside the NDC (nDisplay)\!  
      * Check   
    * 3\) Post Process Volume  
* **Nanite**  
  * Turn Nanite **on** for any static meshes in the level  
  * tbd  
* **Trees**  
  * Build billboard-only trees for background (in Speedtree)  
  * Tbd  
* **Texture Sizes**  
  * Many assets show up with large 4K (4096x4096) textures  
    * This can bog down the GPU and CPU  
  * Solutions  
    * Convert 4K textures to 2K or 1K and re-import  
    * other?
