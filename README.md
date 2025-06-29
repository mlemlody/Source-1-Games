# Source-1-Games

This is the README for Source 1-based games. Source 1-based games include Team Fortress 2, Left 4 Dead 2, and Counter-Strike: Source.

Please use this repository to report bugs and feature requests for Team Fortress 2, Counter-Strike: Source, Left 4 Dead 2, and the Source 1 Engine.

---

## Conduct

There are basic rules of conduct that should be followed at all times by everyone participating in the discussions. While this is generally a relaxed environment, please remember the following:

- Do not insult, harass, or demean anyone.
- Do not intentionally post the same issue multiple times.
- Do not use ALL CAPS when creating an issue report.
- Do not repeatedly update an open issue just to say the problem still persists.

**Remember**: Just because an issue has been reported here does not necessarily mean it is an issue with Team Fortress 2, Counter-Strike: Source, or any other Source 1 game. Also, if your issue is not resolved immediately, that does not mean a resolution is not being researched or tested. Patience is always appreciated.

---

## Reporting Issues

If you encounter a bug while using Source 1 games, first search the [issue list](https://github.com/ValveSoftware/Source-1-Games/issues) to see if it has already been reported. Be sure to include closed issues in your search.

If it has not been reported, create a new issue with at least the following information:

- The game you're reporting the bug on (TF2, CS:S, L4D2, or all)
- A short, descriptive title
- A detailed description of the issue, including any output from the command line
- Steps for reproducing the issue
- Your [system information](#system-information)

Please place logs either in a code block ([GFM cheat sheet](https://guides.github.com/features/mastering-markdown/)) or a [gist](https://gist.github.com).

### System Information

Your system information must include:
- Your Linux distro or OS version
- Your Desktop Environment or Window Manager (Linux only)
- Your graphics card info (manufacturer and model), and all graphics driver versions
- Anything else that might be useful (mouse/keyboard, filesystem type, etc.)

The preferred and easiest way to get this information is from Steam’s Hardware Information viewer in the menu:  
`Help -> System Information`

Once your information appears:  
Right-click within the dialog, choose `Select All`, then right-click again and choose `Copy`.  
Paste this information into your report, preferably in a code block or a [gist](https://gist.github.com).

---

## Feature Requests

If you are asking for a new feature or enhancement for a game, first search the [issue list](https://github.com/ValveSoftware/Source-1-Games/issues) to see if it has already been requested. Be sure to include closed issues in your search.

If it has already been requested, feel free to add your feedback to the existing entry.

If it has not been requested, create a new issue with at least the following information:

- The game you're requesting the enhancement for
- A clear description of what you want
- Justification for why the feature is needed
- Why this feature should be prioritized over others

**Note**: Just because you request a feature doesn't mean it will be implemented. We are primarily focused on fixing existing bugs. That said, your feedback still matters. Be clear. Be concise.

---

## Driver Contact Information

Some issues may stem from video driver problems. Below is a (non-exhaustive) list of where to file bugs or get help:

### AMD

For AMD hardware compatibility and performance issues:  
https://community.amd.com/community/devgurus/steam-linux

For AMD open-source drivers (part of Mesa), refer to the Intel/Mesa links below.

### Intel

Mesa users mailing list (discussions):  
http://mesa3d.org/lists.html

Report bugs and feature requests:  
http://mesa3d.org/bugs.html

### NVIDIA

NVIDIA proprietary drivers:  
https://devtalk.nvidia.com/default/board/98

Open-source Nouveau driver:  
http://nouveau.freedesktop.org/wiki/

If you know of any other useful resources, please let us know.

---

## Known Video Driver / Card Issues

### NVIDIA

NVIDIA 6xxx and 7xxx series GPUs have reached end-of-life (EOL).  
Driver support for these GPUs has been discontinued and the relevant code is no longer compiled.

These GPUs also lack proper sRGB functionality required by Source Engine titles when using OpenGL.  
(Source uses slightly different sRGB behavior under OpenGL compared to the undefined behavior under Direct3D 9, which is why this may work under D3D9 but not OpenGL.)
