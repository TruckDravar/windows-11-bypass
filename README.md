# windows-11-bypass
Bypass TPM 2.0, Secure boot, UEFI, Minimum Ram(4Gb) and Storage(64gb) requirement when installing windows 11

# How to use
> ⚠️**WARNING:** Do steps before trying for error or redo the setup procedure if got one.
1. During Windows 11 installation, when you get the “This PC can’t run Windows 11” message:
    -Press Shift + F10 to open Command Prompt.
2. Type:
    * ``` notepad ```
   and press enter.
4. In Notepad:
   * Paste the code in <pre> ```reg Windows Registry Editor Version 5.00 [HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig] "BypassTPMCheck"=dword:00000001 "BypassSecureBootCheck"=dword:00000001 "BypassRAMCheck"=dword:00000001 "BypassStorageCheck"=dword:00000001 "BypassCPUCheck"=dword:00000001 ``` </pre>
    * Save it as ```windows11-bypass.reg```.
    * File type: ```All Files```.
    * Encoding: ```ANSI```.
5. In Notepad, go to File > Open, right-click your new ".reg" file and Merge it.
