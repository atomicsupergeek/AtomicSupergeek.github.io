# Using ssh to connect to Linux servers
MacOS has a terminal program that comes with the operating system. It is often overlooked by Mac users who often only use graphical applications. However, it is a very powerful tool in the Mac arsenal. 

One of the big uses is to connect to Linux servers using the SSH terminal protocol. You just need to open up terminal, and then SSH to the computer you need to get to. 

## Switching to OpenSSH can make life easier
Apple uses the BSD version of ssh by default. There are a few limitations to this version of ssh. You can install OpenSSH instead. This will make a number of things work better when using ssh in the Mac Terminal program. 

One of the biggest benefits is that you can use a Yubikey, or other FIDO2 key, that supports the PIV protocol to store your private key for public/private key logins. This is one of the most secure ways to access Linux servers. 

The challenge is that Apple uses the BSD implementation of SSH. This version has some features missing. This causes issues with some of the advanced features, like using the PIV protocol for public/private key logins. This is why I now immediately install OpenSSH, and reconfigure my Mac computers to use that instead of the native SSH program. 

## Installing OpenSSH with homebrew
There are a number of benefits of using homebrew to install software on a Mac. You might need to install homebrew first if you have not used it yet. 