# Installation on Windows

## Using Chocolatey
Once you install chocolatey, you can simply run the following command to install Lua
```shell
choco install lua
```
## Using Scoop
Once you install scoop, you can simply run the following command to install Lua
```shell
scoop install lua
```

# Installation on MacOS

## Using homebrew
Install homebrew if you haven't already. Once you have homebrew installed, simply run the following command to install lua

```shell
brew install lua
```

# Installation on Linux

## For Debian/Ubuntu/ based distributions
_This also includes linux mint, pop os, zorin os, and more. If you are not sure if your distro is ubuntu/debian based, search up "is (your distro) ubuntu/debian based._

Open your terminal and update the package lists.
```shell
sudo apt update
```
To install Lua, simply run this command:
```shell
sudo apt install lua
```

If you get an error or output like this:
```shell         
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package lua is a virtual package provided by:
  lua5.4:i386 5.4.6-3build2
  lua5.3:i386 5.3.6-2build2
  lua5.2:i386 5.2.4-3build2
  lua5.1:i386 5.1.5-9build2
  lua5.4 5.4.6-3build2
  lua5.3 5.3.6-2build2
  lua5.2 5.2.4-3build2
  lua5.1 5.1.5-9build2
You should explicitly select one to install.

E: Package 'lua' has no installation candidate
```

Then simply install the latest version you see. For example, the latest version on the output I have is lua5.4, so I would run the following command:

```shell
sudo apt install lua5.4
```
## For fedora based distributions
_If you are not sure if your distro is fedora based, search "is (your distro) fedora based?"_

Open your terminal and simply run the following command:
```shell
sudo dnf install lua
```
## For arch based systems
_This includes Manjaro, EndeavourOS, Garuda Linux, ArcoLinux, CachyOS, Artix, and more. If you are not sure if your distro is arch based, search "is (your distro) arch based"?_

Open your terminal and run the following command:
```shell
sudo pacman -S lua
```

# Building from source with Linux or MacOS (advanced)
If you want to build from source and get the latest version of lua, follow the instructions below.

Firstly, install the necessary development tools like build-essential, libreadline-dev, and/or others.

Use curl or another application to download the latest version of the source code. At the time of writing this, the latest version of lua is 5.5
```shell
curl -L -R -O https://www.lua.org/ftp/lua-5.5.0.tar.gz
```
Extract the archive file and navigate to the directory

```shell
tar zxf lua-5.5.0.tar.gz
cd lua-5.5.0
```

Build and install the source code
```shell
make all install
```
You might need superuser/admin permissions

```shell
sudo make all install
```
# Verify installation (all platforms)
Open your terminal/command prompt and type "lua" in it.
```shell
lua
```
If you see an output that looks similar to this:
```shell
Lua 5.4.6  Copyright (C) 1994-2023 Lua.org, PUC-Rio
> 
```
That means Lua has been installed successfully!