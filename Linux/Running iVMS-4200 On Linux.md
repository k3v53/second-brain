---
tags:
  - Linux
  - Wine
  - Lutris
status: Investigating
aliases:
  - Running iVMS-4200 With Wine
---
I've managed to get it running with the following steps
1. Create a [[Wine Prefix]] (or use the default)
2. Run [[Winetricks]] with the following command: 
 ```bash
 winetricks -q vcrun6sp6 mdac28 mfc42 vlc
 ```
 This will install the necessary dependencies for iVMS-4200 to run.
 3. Execute [the installer](https://www.hikvision.com/en/support/download/software/ivms4200-series/) and install normally.
 4. After that a desktop icon should appear and you've successfully installed 
# Sources
- https://ubuntuforums.org/showthread.php?t=2403886
	- https://www.youtube.com/watch?v=3YDzMtvGUGI
- 