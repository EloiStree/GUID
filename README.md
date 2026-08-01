# GUID

I am a teacher 😋 building [CodeLabTV](http://github.com/EloiStree/CodeLabTV) and [GOMI](http://github.com/EloiStree/GOMI).   

I want to be able to say:   

> You can open this demo using the following code, or alias.   

If you want to use it you can look at those toolboxes:   
- https://github.com/EloiStree/2026_07_31_gdp_load_scene_by_guid   
- https://github.com/EloiStree/2026_01_03_gdp_input_to_primitive   
  
If the demo is present in the build, it will open automatically.   

This allows me to avoid having menus in my game. Instead, I only need an ID to load a demo from:   
* a scanned barcode,
* a QR code,
* the clipboard,
* a fast-typing hardware device,
* or a UDP message such as `LOAD_LEVEL:GUID`.

To use this tool, simply add a file named `guid.txt` to your project with the following format:    
* **First line:** the GUID
* **Second line:** the button title
* **Third line:** a one-line description of the demo
* **Remaining lines:** the Rich BBCode description displayed for the demo

There should be only **one scene** associated with each `guid.txt` file to load.    

Since the documentation for a demo can become much larger than what Rich BBCode is suitable for, you can create a GitHub repository using the scene's ID and store the documentation there, just as I am doing here.     

The goal of this approach is:   
* to create small, isolated demos,   
* to keep documentation that explains how to rebuild a scene and its purpose if it ever breaks.    

You can generate 256-bit GUIDs and their corresponding QR codes here:     
https://eloistree.github.io/Website/static_vibe/guid58/      

Example:    
https://eloistree.github.io/GUID/HelloWorld/    
