
This is a guide on how to install the Vox Populi Mod for Civilization V on Linux easily

Contrary to other guides, this guide doesn't require Lutris, Bottles or any other such program. Only Steam and a program called ProtonTricks is required.
I came with the idea to do it this way because the other solutions didn't quite work for me but that doesn't mean they are invalid of course.

Some other handy links:
https://gitlab.com/baaard/vox-populi-on-linux/-/blob/main/README.md
https://forums.civfanatics.com/threads/vox-populi-on-linux.673879/page-2

If you have any problems, please make an issue and I will try to help

Step 1: Installation of the Windows version of Civ 5
- Open Steam (on your Linux desktop, no Lutris) and right click on Civilization V.
- Click on Compatibility and check the "force compatibility" box. In the dropdown, select either the newest version of proton or proton experimental. Either will work.
- Only now install it (or wait for the update if you had the Linux version before)
  -  (Note: reports suggests that the proton version works better anyway)


Step 2: Installing Vox populi
- Install [Protontricks](https://github.com/Matoking/protontricks). It is available as a Flatpak so you should be able to install it.
- Download the [Vox Populi Automatic Installer](https://forums.civfanatics.com/threads/community-patch-how-to-install.528034/)
- Once downloaded, right click on the executable and select open with -> protontricks
- Select Civilization V, click OK and wait for a bit. After a few seconds the install window should pop up
- The default install location is still valid since the exe file is loaded within the environment (wine prefix) of Civ 5
- Click next and close the window in the end

Step 3: A small hack
You would think VP is installed but there is a small problem. VP installs the mods in the mod directory (the one that was selected) but also installs some textures in the default steam install location. The problem is that Civ5 is not there.

- 3a
  - Open Protontricks and select Civ 5. You can safely ignore the warning about 64-bit prefixes
  - Select "Select the default prefix" and click on OK
  - In the next window, select "browse files" and hit OK. A new window or tab should open in your file manager (check because with Wayland the app is not     brought to the foreground). 
  - You can close the Protontricks window(s)

- 3b
  -  navigate to "some_directory/drive_c/Program Files (x86)/Steam/steamapps/common/Sid Meier's Civilization V/" where some directory is the path where Protontricks sent you. The path will look something like this: "~/.local/share/Steam/steamapps/compatdata/8930/pfx/drive_c/Program Files (x86)/Steam/steamapps/common/Sid Meier's Civilization V/
  -  Copy the contents of the folder. At the time of writing, this is only the "Assets" folder.
  -  Paste the folder in the installation location of Civ 5 of Steam. The default location is: "~/.local/share/Steam/steamapps/common/Sid Meier's Civilization V/"


Step 4: Enjoy the game!
