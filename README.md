# img2cons
Visualizes images insice of the terminal.
## How to use
### Compiling
Simply use your favorite c-compiler to compile ```img2cons.c```, e.g.:
```
  gcc -o img2cons img2cons.c
```
### Running 
```
  // display multiple images
  img2cons <file1> <file2> ...
  // specify specific image width (defaul 32) , the height will be proportional
  img2cons -w 16 <file1> <file2> -w 64 <file3>...
  // print the help dialog
  img2cons --help
```
## Enable color printing on windows
Color printing using escape codes is often disabled by default.
To enable either run the ```win_enable.bat``` file, which runs:
```
  reg add HKEY_CURRENT_USER\Console /v VirtualTerminalLevel /t REG_DWORD /d 0x00000001 /f
```
To remove, run ```win_disable.bat```.