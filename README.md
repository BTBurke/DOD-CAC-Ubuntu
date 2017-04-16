Using DOD CAC on Ubuntu
===

This was verified to work on Ubuntu 16.10 with Firefox 52.0a2 developer edition (15 Apr 17).

Super simple:

1. Follow the instructions on the Ubuntu community wiki: https://help.ubuntu.com/community/CommonAccessCard
2. Install cackey from this repository
	* This is the package from Forge.mil, included here for ease of installation since Forge.mil requires a working CAC to download
3. If you have trouble installing the DEB via dpkg, open it with archive manager and extract the data.tar.gz file, then copy libcackey.so to the /usr/lib directory.
4. Configure Firefox by going to Preferences -> Advanced -> Security Devices then selecting Load and point it to the libcackey.so file.
