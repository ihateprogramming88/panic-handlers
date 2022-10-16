# panic-handlers

Panic handlers I wrote for my Qubes system

They wipe the system's LUKS headers before shutdown to ensure data is irrecoverable. They also perform TRIM to encourage the drive to actually zero old blocks

These scripts were designed to run on Qubes inside dom0, but should work on most Linux-based OSs. On XFCE systems, this script also locks the screen to prevent interrupting the panic process

### How to copy files to dom0

The Qubes official documentation has information about copying files to dom0: https://www.qubes-os.org/doc/how-to-copy-from-dom0/#copying-to-dom0

For the best security, you should download this into a disposable VM, to prevent a compromised qube from tampering with the data locally
