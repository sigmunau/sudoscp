# sudoscp
## About

sudoscp is a short script to allow copying files that are not readable or writable by your user between machines where you have sudo access but don't have access to log in as root over ssh.
The servers does not need to be able to reach each other. No temporary files are written on either servers nor on the box the script is running from.

## Prereq

Both servers need to be accessible by passwordless ssh (using public key auth). Both servers need to have `tar` and `sudo` installed.
