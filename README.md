# code-server port for FreeBSD

## code-server has become a part of the ports tree

code-server is now officially available in the FreeBSD ports tree. For more information, please see the following URL:

- https://www.freshports.org/www/code-server/

This git repository serves as the public development repository for the FreeBSD code-server port.

---

This repository contains the FreeBSD port of code-server.

code-server allows you to run Visual Studio Code in a web browser and access a development environment remotely.

# Build

Install directly from the FreeBSD package repository:

```shell
pkg install code-server
```
or:

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

## Extension Compatibility

Since version 4.135.0_1 the port installs extensions from the Open VSX
registry as on any other platform (earlier versions rejected most
extensions because of a platform detection issue).

Extensions that bundle native Linux binaries (language servers, debug
adapters) need the native FreeBSD tool from ports and a one-line
setting. See [EXTENSIONS.md](EXTENSIONS.md) for verified recipes and
the known limitations (Pylance, C/C++ and Live Share are licensed for
Microsoft builds only and cannot be supported).

## Platform

- Built on FreeBSD 14 amd64
- Built on FreeBSD 15 amd64
- Built on FreeBSD 16 amd64

---

If you like my work, consider sponsoring me on [GitHub Sponsors](https://github.com/sponsors/joneum/).
