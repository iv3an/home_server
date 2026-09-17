# Proxmox Security Homelab

A personal Proxmox-based home server built as a hands-on environment for learning Linux administration, virtualization, networking, and defensive security.

The lab runs on a dedicated private network and is managed from my Windows laptop using the Proxmox web interface and SSH.

## Architecture

```text
Dorm Wi-Fi
     |
     v
Lab Router
     |
     +----------------------+
     |                      |
Windows Laptop        Proxmox Server
                            |
              +-------------+-------------+
              |             |             |
         Ubuntu Server  Windows Server   Kali Linux
              |             |
           Docker      Active Directory
              |
           Pi-hole

Security Logs
     |
   Sysmon
     |
   Splunk
```

## Lab Goals

* Learn Proxmox virtualization
* Improve Linux system administration skills
* Practice SSH and remote server management
* Understand TCP/IP, DNS, and local networking
* Build and manage Windows Server and Active Directory
* Deploy self-hosted services with Docker
* Collect and analyze logs
* Build a small SOC-style security monitoring environment

## Current Progress

* [x] Dedicated lab router configured
* [x] Private LAN created
* [ ] Proxmox VE installed
* [ ] SSH configured
* [ ] Ubuntu Server VM created
* [ ] Docker configured
* [ ] Pi-hole deployed
* [ ] Windows Server deployed
* [ ] Active Directory configured
* [ ] Sysmon configured
* [ ] Splunk deployed
* [ ] SOC monitoring lab completed

## Planned Services

### Ubuntu Server

Used for Linux administration, SSH, Docker, networking experiments, and security tooling.

### Pi-hole

Network-wide DNS filtering and a practical environment for learning DNS traffic and network visibility.

### Windows Server

Used to build an Active Directory environment with users, groups, Group Policy, and domain-joined clients.

### Splunk + Sysmon

Used to collect Windows events and practice basic SIEM monitoring and security investigation.

### Kali Linux

An isolated VM used for testing and generating security events inside the lab environment.

## Documentation

Detailed documentation will be added as the lab develops:

* [Proxmox Installation](setup/proxmox-installation.md)
* [Network Configuration](setup/networking.md)
* [SSH Setup](setup/ssh-setup.md)
* [Pi-hole](services/pihole.md)
* [Windows Server](services/windows-server.md)
* [Active Directory](services/active-directory.md)
* [Splunk](services/splunk.md)
* [Sysmon](security-lab/sysmon.md)

## Skills Practiced

`Proxmox` `Linux` `SSH` `Networking` `Docker` `DNS` `Windows Server` `Active Directory` `Sysmon` `Splunk` `SIEM` `Blue Team`

## Project Status

This homelab is actively being built and documented as I learn new technologies and security concepts.
