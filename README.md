PLEASE READ THIS!!!!!!!!!!!
==================
This is a forked version of the pf2ad utility which allows you to install Samba packages on a server running pfSense 2.4.3. Please note that this script has been updated to work with the latest pfSense version 2.5.1 - RELEASE. That being said we have not yet tested it fully. Please use this script at your own risk and pay attention to any output that is created in order to submit bug reports for us to resolve.

~ Sam (nano)


How to install
==================

The script is automatic, meaning you need not install anything, he will have to check the necessary dependencies and install the needed.

To make the application of change patches and NTLM authentication setting in pfSense® software, we will need version 2.4.3 of pfSense® software. Remember that this version is compatible (will install if you have not) with Squid package, you will need web access or console (recommend using the console via ssh to monitor the process).

```bash
fetch -q -o - https://raw.githubusercontent.com/nano11bravo/pf2ad/2.5.1-SAMBA4/pf2ad.sh | sh
```

It will upgrade the system package, add a custom repository with samba version with AD support, will if necessary the installation of the dependent packages (Squid), apply changes to the Squid package code and the system menu to add configuration options of AD authentication.


