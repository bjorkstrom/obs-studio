BUILD OBS
=========

Reference: https://github.com/jp9000/obs-studio/wiki/Install-Instructions#windows-build-directions

- Download QT
  - Install 5.9.2
- Download depencies for OBS:
  - https://obsproject.com/downloads/dependencies2015.zip

-
  >mkdir OBS
  >cd OBS
  >git clone --recursive https://github.com/jp9000/obs-studio.git
  >mkdir build
  >cd build
  >cmake-gui ..

  - Press "Configure"
  - Choose mvs 2015 and x64.
  - Set obs depency path to where you unpacked them.
  - Set QT5.9.2 dir.
  - Press "Configure" again.
  - Press Generate and quit.

- Open the solution file in build dir.
- Set release and x64 configuration.
- Build all.

- Copy dir build/rundir/Release to Assets/StreamingAssets/Obs/
  You need to copy all including subdirs bin/ data/ and obs-plugins/
