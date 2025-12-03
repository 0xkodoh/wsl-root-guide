# WSL Root Access Guide

This repo explains how to switch to the root user in WSL, how to launch WSL directly as root, and how to set root as the permanent default user. It also covers optional prompt customization.

## Table of Contents
- Check your WSL distro name
- Switch to root temporarily
- Launch WSL as root (one-time)
- Set root as default user (permanent)
- Revert default user
- Customize the root prompt
- Screenshots

## Check your WSL distro name
```powershell
wsl -l -v
```

## Switch to root temporarily
```bash
sudo su
```

## Launch WSL as root (one-time)
```powershell
wsl -d <DistroName> -u root
```

## Set root as default user (permanent)
```powershell
ubuntu2404.exe config --default-user root
```

## Revert default user
```powershell
ubuntu2404.exe config --default-user kodo
```

## Customize the root prompt
```bash
sudo nano /root/.bashrc
PS1="root@847839:\w$ "
source /root/.bashrc
```

## Screenshots
Place images inside the screenshots folder.
