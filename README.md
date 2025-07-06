# BlackBoot

This program overwrites the Master Boot Record (MBR) of the primary physical drive (`PhysicalDrive0`) with a custom bootloader message.

**Warning:** This program will corrupt the boot sector and make your system unbootable. Use only in a virtual machine or controlled environment

## Important Notice

The source code will **not** be publicly shared to avoid misuse and prevent skids from spreading harmful copies that can damage systems.

## How it works

- Writes 512 bytes to the MBR with a small bootstrap code.
- Displays the message:  
  `YOUR PC HAS BEEN TRASHED LIL KID`
- Sets the correct boot signature (`0x55 0xAA`) at the end.
- Requires administrator privileges to run.
