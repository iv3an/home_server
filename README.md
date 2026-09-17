# Proxmox Security Homelab

A personal Proxmox-based home server built as a hands-on environment for learning Linux administration, virtualization, networking, self-hosting, and defensive security.

The lab runs on a dedicated private network and is managed from my Windows laptop using the Proxmox web interface and SSH.

## Architecture

```text
 PUBLIC / DORM LAN
        |
        v
    Lab Router
        |
        +----------------------+
        |                      |
Windows Laptop          Proxmox Server
                              |
        +---------------------+----------------------+
        |                     |                      |
   Ubuntu Server          Containers              Kali VM
        |                     |                      |
      Docker               Pi-hole              Security Labs
        |                Home Assistant
        |                   Immich
        |
   +----+---------+
   |              |
Minecraft       Other
Server          Services

        +---------------------+
        |                     |
       NAS              Backup Server
```

## Lab Goals

* Learn Proxmox virtualization
* Improve Linux system administration skills
* Practice SSH and remote server management
* Understand TCP/IP, DNS, and local networking
* Learn Docker and container management
* Host and manage self-hosted services
* Gain experience with storage and backups
* Build hands-on defensive security skills

## Current Progress

* [x] Dedicated lab router configured
* [x] Private LAN created
* [ ] Proxmox VE installed
* [ ] SSH configured
* [ ] Ubuntu Server VM created
* [ ] Docker configured
* [ ] Pi-hole deployed
* [ ] Minecraft server deployed
* [ ] NAS configured
* [ ] Immich deployed
* [ ] Home Assistant deployed
* [ ] Backup server configured
* [ ] Kali Linux VM deployed

## Planned Services

### Ubuntu Server

Used for Linux administration, SSH, Docker, networking, and self-hosted applications.

### Minecraft Server

Modded Minecraft server used to practice Linux server management, networking, resource management, and service hosting.

### NAS

Network-attached storage for personal files, media, server data, and backups.

### Pi-hole

Network-wide DNS filtering used to learn more about DNS, network traffic, and local services.

### Immich

Self-hosted photo and video management platform for building a personal cloud photo library.

### Home Assistant

Self-hosted home automation platform used for experimenting with local services and integrations.

### Backup Server

Used to store backups of virtual machines, containers, configurations, and important server data.

### Kali Linux

An isolated VM used for cybersecurity labs, network testing, and defensive security practice.

## Skills Practiced

`Proxmox` `Linux` `SSH` `Networking` `Docker` `Containers` `DNS` `Pi-hole` `NAS` `Virtualization` `Self-Hosting` `Kali Linux`

## Project Status

This homelab is actively being built and expanded as I learn more about virtualization, Linux, networking, self-hosting, and cybersecurity.
