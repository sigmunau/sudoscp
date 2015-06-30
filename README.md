# sudoscp
## About

sudoscp is a short script to allow copying files that are not readable or writable by your user between machines where you have sudo access but don't have access to log in as root over ssh.
The servers does not need to be able to reach each other. The files to copy are not written to temporary files on either servers nor on the box the script is running from.

## Example

```
sudoscp server1.example.com server2.example.com /tmp/myfile /tmp/myfile2
Enter Password:
/tmp/myfile
/tmp/myfile2
```

## Prereq

Both servers need to be accessible by passwordless ssh (using public key auth). Both servers need to have `tar` and `sudo` installed. The sudo password needs to be the same on both servers.
