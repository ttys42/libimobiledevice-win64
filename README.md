# libimobiledevice-win64
An easy-to-build, Visual Studio 2015 compatible version of the latest Libimobiledevice for 64-bit Windows.

# Instructions
- Clone, go into the `libimobiledevice-windows` directory
Get openssl from http://slproweb.com/products/Win32OpenSSL.html; you need both 32 bit and 64 bit installers, 
e.g., Win32 OpenSSL v1.0.1j and Win64 OpenSSL v1.0.1j. Run the installers and choose the location as 
libimobiledevice-windows\OpenSSL-Win32 or libimobiledevice-windows\OpenSSL-x64. NOTE: THE 64 BIT INSTALLER 
INSTALLS TO OpenSSL-Win64 BY DEFAULT. THIS MUST BE CHANGED TO OpenSSL-x64 (in the libimobiledevice-windows
directory). Also choose to copy the OpenSSL directories to /bin directory.

Your libimobiledevice-windows directory should have the following sub-directories:

lib
libcnary
libgen
libiconv
libxml2
OpenSSL-Win32
OpenSSL-x64
vendors

- Finally, open the `.SLN` with VS2015, and build.

This project's source code comes from [https://github.com/libimobiledevice/libimobiledevice](https://github.com/libimobiledevice/libimobiledevice), a version specifically for Linux that is quite difficult to build on Windows, even with Cygwin. This project includes modifications from Polyfun.

The official Libimobiledevice is licensed under GPL and LGPL.
