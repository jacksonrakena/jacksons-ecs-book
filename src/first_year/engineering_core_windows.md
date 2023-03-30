# Setting up Geany and WSL on Windows systems
*Guide written by [Jackson](https://github.com/jacksonrakena) with help and pictures from [Gold](https://github.com/goldsolitude)*

This guide details how to install MinGW/clang, and ENGR 101's preferred code editor, Geany, on a Windows or macOS operating system. Linux users (who probably don't need any guide) should follow the guide on the ECS wiki.

If you've already got mingw/clang installed, skip to the bottom to install Geany.

# Installing MinGW (or clang)

This guide details how to install MinGW, the GNU C/C++ compiler, on a Windows or macOS operating system (`clang`).

### Mac
If you have a Mac, you'll probably need to run `xcode-select -install` in a Terminal window, and wait for it to finish, and then you should be done. (This will install Clang, which is GCC-compatible)

### Windows
If you have anything in `C:\MinGW`, delete it.

1) Go to [this website](https://techdecodetutorials.com/download/) and click either `MinGW C/C++ For Windows 11 32/64 bit` (for Windows 11) or `MinGW C/C++ For Windows 10 32/64 bit` (for Windows 10)  
**Do not download the Turbo compiler.**
1) Run the downloaded file (`mingw.exe`). When it asks for a path, enter `C:\MinGW`. 
2) Click 'Extract'. Wait.
3) In Windows search, type 'env' and click on 'Edit the system environment variables'.  
4) Click the entry for 'Path' and click 'Edit'.  
5) Click 'New', and type `C:\MinGW\bin`.
6) Click 'ok' and close all the windows.
7) Open `Command Prompt` and type `g++ --version`
(you may need to restart Command Prompt if you had any open windows)

If you still can't make it work, attend an ENGR 101 Workshop session.

# Installing Geany
Install Geany from [https://www.geany.org/download/releases/](https://www.geany.org/download/releases/).

<img width="418" alt="image" src="https://user-images.githubusercontent.com/44521335/156319649-c3a55e8c-cded-4224-8cde-ab8eae88c6c3.png">
 
Choose the right option from the table below:  
  
| Operating System      | Download       |
|---------|-------------------------------------------------------------|
| Windows | `geany-{version}_setup.exe`                                 |
| Apple, Intel processor | `geany-{version}_osx-4.dmg`                  |
| Apple, Apple Silicon processor (M1/M2) | `geany-{version}_osx_arm64.dmg` |
  