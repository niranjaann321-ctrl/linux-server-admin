# Week 1 Journal

## Objectives

- Install Ubuntu Server
- Configure VirtualBox
- Configure SSH remote administration
- Configure networking

---

# Virtual Machine Setup

Installed Ubuntu Server 26.04 LTS using Oracle VirtualBox.

Configuration:
- RAM: 4096 MB
- CPU: 2 cores
- Storage: 25 GB
- Network:
  - NAT Adapter
  - Host-only Adapter

---

# OpenSSH Configuration

Installed OpenSSH Server during Ubuntu installation.

Verified SSH service using:

```bash
sudo systemctl status ssh
```

Successfully connected remotely using:

```bash
ssh ubuntuuser@192.168.56.101
```

---

# Network Configuration

## IP Address

```bash
ip addr
```

Server IP:
```text
192.168.56.101
```

---

# System Information

## Kernel

```bash
uname -a
```

## Memory

```bash
free -h
```

## Disk

```bash
df -h
```

## Ubuntu Version

```bash
lsb_release -a
```



# Problems Faced

## Time Synchronization Issue

The VM time was incorrect which caused apt update failures.

### Solution
- Restarted VM
- Corrected time synchronization
- Re-ran updates

---

# Reflection

This week I learned:
- Linux server installation
- SSH remote administration
- VirtualBox networking
- Command-line administration
- Basic troubleshooting
