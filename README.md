# Simple Shell Injection

Simple C program which uses the Win32 api to get a process handle to "notepad.exe" and injects shell code to open "mspaint.exe"

Written as a study of the video [Malware Development: Process Injection](https://youtu.be/A6EKDAKBXPs?si=3spdld4GohzW5a4g).

The shell code data was gotten from the [Metasploit Framework](https://docs.metasploit.com/).

To compile:

1. Install the [Windows SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/) to get access to the `windows.h` header
2. Run your compile tool (tested using [gcc](https://gcc.gnu.org/)).

## Obs
Your AV may freak out, so if you want to run it you will need to disable it (even if you use only the Windows Defender).

Windows Defender will also delete the file as soon as it's compiled, so you may want to add the folder as an exclusion in the configurations.
