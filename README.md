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

# Proxmox Security Homelab

A personal Proxmox-based home server built as a hands-on environment for learning Linux administration, virtualization, networking, self-hosting, and defensive security.

The lab runs on a dedicated private network and is managed from my Windows laptop using the Proxmox web interface and SSH.

---

## Overview

The server acts as the main platform for running virtual machines, containers, storage, and self-hosted applications.

### Planned Services

* Modded Minecraft server hosting
* Network-Attached Storage (NAS)
* Pi-hole DNS filtering
* Immich photo and video server
* Home Assistant
* Backup server
* Docker-based applications
* Kali Linux security lab

### Key Goals

* Learn Proxmox virtualization and container management
* Improve Linux system administration skills
* Become more comfortable working from the command line
* Practice SSH and remote server administration
* Gain hands-on experience with TCP/IP, DNS, and local networking
* Learn storage, file sharing, and backup management
* Experiment with useful self-hosted services
* Build practical defensive security and infrastructure skills

The main purpose of this server is to act as a long-term learning environment where I can build, break, troubleshoot, and improve real services.

---

## System Information

* **Hypervisor:** Proxmox VE
* **Primary Management Device:** Windows laptop
* **Remote Management:** SSH
* **Web Management:** Proxmox Web Interface
* **Network:** Dedicated private LAN
* **Virtualization:** Virtual Machines and Linux Containers
* **Containers / Applications:** Docker where appropriate

Proxmox runs directly on the server hardware and is used to manage the virtual machines, containers, storage, networking, and server resources.

---

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

---

## Network Configuration

The homelab uses a dedicated router to create a private network separate from the main network.

### Private LAN

* Proxmox server connected to the lab router
* Windows laptop used to access and manage the server
* Local IP addressing for internal services
* Services remain inside the lab network unless remote access is intentionally configured

### DNS

Pi-hole is planned as the lab's DNS filtering service to provide:

* Network-wide DNS filtering
* DNS request visibility
* Local networking practice
* Experience configuring DNS clients and servers

---

## Remote Access & Management

### SSH

SSH is the primary method for managing Linux systems from my Windows laptop.

Planned configuration includes:

* SSH key authentication
* Remote command-line administration
* Secure file transfers
* Managing services without requiring a graphical interface

### Proxmox Web Interface

The Proxmox web interface is used to manage:

* Virtual machines
* Containers
* Storage
* Networking
* Backups
* Server resources
* Snapshots

---

## Services & Workloads

### Minecraft Server

A Minecraft server used to gain practical experience with:

* Linux service hosting
* Resource allocation
* Networking
* Server configuration
* Monitoring and troubleshooting

### NAS

Network-attached storage used for:

* Personal files
* Media
* Server data
* Backups

The NAS will also provide hands-on experience with Linux storage, permissions, and network file sharing.

### Pi-hole

Network-wide DNS filtering service used to block unwanted domains and learn more about DNS and network traffic.

### Immich

Self-hosted photo and video management platform used as a personal alternative to cloud photo services.

### Home Assistant

Self-hosted automation platform used to experiment with locally managed services, integrations, and automation.

### Docker

Docker is used where containerized deployment makes sense.

It provides a lightweight way to deploy and manage selected applications without creating a full virtual machine for every service.

### Kali Linux

An isolated Kali Linux VM used for:

* Cybersecurity labs
* Network testing
* Security tools
* Generating and analyzing activity inside the homelab

### Backup Server

Dedicated storage for:

* Virtual machine backups
* Container backups
* Configuration files
* Important server data

---

## Server Management & Tooling

Tools used or planned for managing the lab include:

* **SSH** — Remote Linux administration
* **Proxmox VE** — Virtualization and infrastructure management
* **Docker** — Containerized applications
* **Linux CLI** — Primary server administration environment
* **Git / GitHub** — Configuration and project documentation
* **Network utilities** — Troubleshooting DNS, connectivity, and services

---

## Operational Approach

* Linux and CLI-focused administration
* Use VMs and containers depending on the workload
* Keep services organized and isolated
* Avoid unnecessary public exposure of internal services
* Maintain backups of important systems and data
* Document configurations, problems, and solutions
* Use the lab for practical learning rather than only following tutorials

---

## Current Progress

* [x] Dedicated lab router configured
* [x] Private LAN created
* [x] Proxmox VE installed
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

---

## Skills Practiced

`Proxmox` `Linux` `SSH` `Networking` `Docker` `Containers` `DNS` `Pi-hole` `NAS` `Virtualization` `Self-Hosting` `Kali Linux`

---

## Project Status

This homelab is actively being built and expanded as I learn more about virtualization, Linux, networking, self-hosting, system administration, and cybersecurity.



