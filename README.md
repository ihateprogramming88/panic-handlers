# panic-handlers

Panic handlers I wrote for my Qubes system

They wipe the system's LUKS headers before shutdown to ensure data is irrecoverable. They also perform TRIM to encourage the drive to actually zero old blocks

These scripts were designed to run on Qubes inside dom0, but should work on most Linux-based OSs. On XFCE systems, this script also locks the screen to prevent interrupting the panic process
