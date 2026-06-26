<p align="center">
  <img src="assets/logo.png" alt="PROJECT_NAME Logo" width="120" height="120">
</p>

<h1 align="center">PROJECT_NAME</h1>

<p align="center">
  A self-hosted Minecraft server hosting panel built for Ubuntu and Docker.
  <br>
  Designed to make running, managing, and deploying Minecraft servers easier without needing a paid hosting provider.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Ubuntu-orange" alt="Ubuntu">
  <img src="https://img.shields.io/badge/Platform-Docker-blue" alt="Docker">
  <img src="https://img.shields.io/badge/Minecraft-Java%20%7C%20Modded%20%7C%20Plugins-green" alt="Minecraft">
  <img src="https://img.shields.io/badge/Status-Active%20Development-yellow" alt="Status">
</p>

---

## Overview

**PROJECT_NAME** is a self-hosted Minecraft server hosting application designed to replicate the convenience of paid Minecraft hosting panels while giving you full control over your own hardware.

It is built to run on a **headless Ubuntu server**, a local machine, or inside **Docker containers**, making it useful for home labs, LAN servers, small communities, IT shops, and anyone who wants a clean way to host multiple Minecraft servers from one device.

The goal of this project is simple:

> Make Minecraft server hosting feel like a professional hosting panel, but self-hosted, flexible, and fully under your control.

---

## Screenshots

> Screenshots will be added here.

### Dashboard

![Dashboard Screenshot](assets/screenshots/dashboard.png)

### Server Console

![Server Console Screenshot](assets/screenshots/console.png)

### Server Manager

![Server Manager Screenshot](assets/screenshots/server-manager.png)

### Modpack / Version Installer

![Modpack Installer Screenshot](assets/screenshots/modpack-installer.png)

---

## Features

### Server Management

- Create and manage multiple Minecraft servers
- Start, stop, restart, and monitor servers
- View live console output
- Send console commands directly from the panel
- Manage server files
- Configure memory, CPU, storage, and startup settings
- Assign ports and server addresses
- View server status from the dashboard

### Docker Support

- Run Minecraft servers inside isolated Docker containers
- Safer separation between servers
- Easier cleanup, redeployment, and migration
- Works well on Ubuntu servers, home labs, and dedicated machines
- Can be used locally or over a network

### Ubuntu Server Support

- Designed for headless Ubuntu installations
- Can be hosted on a spare PC, mini PC, server, or VPS
- Useful for local network hosting or public-facing Minecraft servers
- Built with self-hosting and remote management in mind

### Minecraft Server Types

PROJECT_NAME is designed to support a wide range of Minecraft server software, including:

- Vanilla
- Paper
- Purpur
- Spigot
- Bukkit
- Forge
- NeoForge
- Fabric
- Quilt
- Velocity
- BungeeCord
- Waterfall
- Bedrock-compatible setups
- GeyserMC / Floodgate crossplay setups

### Modpack Support

The project is intended to support modern Minecraft modpack workflows without forcing every server to run unnecessary installers.

Supported or planned platforms include:

- CurseForge
- Modrinth
- FTB
- Technic
- ATLauncher
- Prism / MultiMC-style server packs

The app should be able to detect when a modpack already includes the correct startup files and avoid blindly running a Forge installer when it is not needed.

Examples of startup patterns the app should handle:

```bash
java -jar server.jar
java @user_jvm_args.txt @libraries/net/minecraftforge/forge/.../unix_args.txt
./start.sh
./run.sh
