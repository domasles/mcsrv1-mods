# MC SERVER1

## This repository contains MC Server1 resources

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
git clone https://github.com/domasles/mc-srv1
```
5. Remove the existing mods and resourcepacks directory:
```bash
rmdir /S /Q %appdata%\.minecraft\mods
rmdir /S /Q %appdata%\.minecraft\resourcepacks
```
6. Create a symbolic link to cloned mods and resourcepacks directories:
```bash
mklink /D %appdata%\.minecraft\mods %userprofile%\documents\code\mc-srv1\mods\client
mklink /D %appdata%\.minecraft\resourcepacks %userprofile%\documents\code\mc-srv1\resourcepacks
```

### Updating

1. Navigate to the cloned repository:
```bash
cd %userprofile%\documents\code\mc-srv1
```
2. Pull the latest changes:
```bash
git pull
```
