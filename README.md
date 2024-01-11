# frida-ios-dump for Windows
Same as AloneMonkey's frida-ios-dump, just modified some lines in the Python script to use 7zip.

## Requirements
- same as frida-ios-dump requirements.txt file content.
- for iproxy step mentioned in AloneMonkey's repo, you can use iFred09's iproxy.exe (https://github.com/iFred09/libimobiledevice-windows).

## Notes
- needs to be run as Administrator (as I had some permission problems when running it as unprivileged user).
- during running of frida-ios-dump on an iOS application, the dump also included "libloader.dylib.fid" related to "iGameGod" app which i had on my jailbroken device. this caused some errors so i just ignored it (commented lines 82, 83). This can be useful for you if that's the case so just uncomment it.
