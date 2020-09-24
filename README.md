# avogadro-squared
Avogadro superbuild project, builds Avogadro dependencies and then Avogadro itself

Why does this fork exist?
I recently switched to Ubuntu 20.04 LTS, after many years as a happy Fedora user. Not my first choice but working from home has required me to dedicate my own hardware to my research. I needed CUDA to work properly and Nvidia does officially, and reliably, support Ubuntu.

Alas, Avogadro 1 has been removed and replaced by Avogadro 2. While Avo2 is very good it still lacks certain features I require (and the Linux version is also currently broken in regards to plugins). So the need for this fork.

For compiling on Ubuntu 20.04 LTS.

Must install Qt4 from external repo:
sudo add-apt-repository ppa:rock-core/qt4
sudo apt install qt-dev-tools


Changes I needed to make:
Hardcoded path to zlib-1.2.8 which is no longer accessible. Updated to zlib-1.2.11.
