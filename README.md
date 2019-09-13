# regolith-cubic-conf

This repository holds configuration files and instructions for generating the Regolith ISO installer.

# LiveCD / ISO Release Instructions

1. Install and run Cubic
2. Specify a directory for installation files.
3. Specify Ubuntu ISO for base (currently 19.04).
4. Set versioning info.  Releases beging w/ 'R' followed by major.minor version.  Ex "R1.2".
5. Select Next in the wizard comes the terminal session.
6. Copy whatever login backdrop image needed into the Cubic terminal, and move it to `/usr/share/backgrounds/warty-final-ubuntu.png`
7. Add the Ubuntu "Universe" repo: `add-apt-repository universe`
8. Add the Regolith repo: `add-apt-repository ppa:kgilmer/regolith-stable`
9. Install Regolith: `apt install regolith-desktop`
10. Install the Regolith gdm3 theme: `apt install regolith-gdm3-theme`
11. Go to next, remove libreoffice* and rythmbox* from the Package Manifest
12. In ISO boot configurations, replace "Ubuntu" with "Regolith" on all tabs.
13. Click 'Generate' to make the ISO image.

