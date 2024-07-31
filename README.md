# Download GraalVM
A simple powershell script to download a specific GraalVM Java distribution, written for the convenience of Luna Pixel Studios' users.

## Table of Contents

- [Usage](#usage)
- [Common Issues](#issues)

## Usage

### Fast Method
1. Right click the Windows icon at the bottom left of your screen.
2. Click "Windows Powershell"
3. Copy the following text: `irm https://raw.githubusercontent.com/chorbintime/download-graal/main/download_graal.ps1 | iex`
4. Paste it into the Powershell window
5. Answer the questions you're given on screen

### Alternate Method
1. Download the file [download_graal.ps1](https://github.com/chorbintime/download-graal/releases/download/release/download_graal.ps1) to your system.
2. Right click on the file and press "Run with PowerShell"
3. Answer the questions you're given on screen

## Issues
It's possible your system may not allow you to run the script. This is a Windows 11 "security" feature that must be circumvented. There are two solutions to this, a temporary one that will work on only one file (in this case mine), or a permanent script that will make it possible to run all scripts you download. The choice is yours.

### Temporary Fix
- Open PowerShell and run the snippet below
```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File C:\Users\YOUR_USERNAME\Downloads\download_graal.ps1 # replace the `-File` path with your own file path
```

### Permanent Fix
- Open PowerShell with Administrator privileges and run the snippet(s) below
```powershell
Set-ExecutionPolicy RemoteSigned
Unblock-File -Path C:\Users\YOUR_USERNAME\Downloads\download_graal.ps1 # not necessary always but sometimes
```

## License
This project is licensed under the GNU GPL v3 License. Please be mindful of this when forking, sharing, and redistributing the software.
