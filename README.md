# MC SERVER1 MODS

## This repository contains MC Server1 mods

### Installation

1. Install Git:
```bash
winget install --id Git.Git -e
```
2. Create a directory for the code:
```bash
mkdir %userprofile%\documents\code
```
3. Navigate to the code directory:
```bash
cd %userprofile%\documents\code
```
4. Clone the repository:
```bash
git clone https://github.com/domasles/mcsrv1-mods
```
5. Remove the existing mods directory:
```bash
rmdir /S /Q %appdata%\.minecraft\mods
```
6. Create a symbolic link to the cloned mods directory:
```bash
mklink /D %appdata%\.minecraft\mods %userprofile%\documents\code\mcsrv1-mods\client
```

### Updating

1. Navigate to the cloned repository:
```bash
cd %userprofile%\documents\code\mcsrv1-mods
```
2. Pull the latest changes:
```bash
git pull
```
