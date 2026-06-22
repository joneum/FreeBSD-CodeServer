# code-server port for FreeBSD

## code-server has become a part of the ports tree

code-server is now officially available in the FreeBSD ports tree. For more information, please see the following URL:

- https://www.freshports.org/www/code-server/

This git repository serves as the public development repository for the FreeBSD code-server port.

---

This repository contains the FreeBSD port of code-server.

code-server allows you to run Visual Studio Code in a web browser and access a development environment remotely.

## Get

Install directly from the FreeBSD package repository:

```shell
pkg install code-server
```

# Build

Build and install code-server from the FreeBSD Ports Collection:

```shell

cd /usr/ports/www/code-server

make install clean

```

Alternatively, clone this repository and build the port directly:

```shell

git clone https://github.com/joneum/FreeBSD-CodeServer.git

cd FreeBSD-CodeServer/www/code-server

make install clean

```
```

## Extension Compatibility

Not all Visual Studio Code extensions currently work on FreeBSD.

Some extensions contain platform-specific binaries or officially support only Linux, macOS, and Windows. While many extensions work without modification, others may require additional patching or may not work at all.

## Platform

- Built on FreeBSD 14 amd64
- Built on FreeBSD 15 amd64
