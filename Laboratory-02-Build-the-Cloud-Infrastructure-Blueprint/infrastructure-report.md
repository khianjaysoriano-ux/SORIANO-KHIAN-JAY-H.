
# Cloud Infrastructure Assessment Report

## General System Information
* **Hostname:** `ubuntu`
* **IP Address:** `172.30.1.2 172.17.0.1`
* **Operating System:** Ubuntu Linux (64-bit)
* **Kernel / Architecture:** `x86_64`

---

## Compute Infrastructure Details
* **CPU Architecture:** `x86_64` (32-bit, 64-bit op-modes)
* **CPU Model Name:** Intel Xeon E312xx (Sandy Bridge, IBRS update) @ 2.0GHz
* **Total CPU Cores:** 1 Core
* **Virtualization Type:** KVM (Full Virtualization)
* **Total RAM:** 1.9 GiB
* **RAM Currently Used:** 415 MiB
* **RAM Currently Available:** 1.5 GiB

---

## Storage & File System Assessment
* **Primary Disk Partition:** `/dev/vda1` (Mounted on `/`)
* **Total Storage Size:** 19 GB
* **Used Storage:** 5.4 GB (30%)
* **Available Storage:** 13 GB
* **Boot Partition Size:** 881 MB (`/dev/vda16`)

---

## Terminal Output Summary

```text
root@ubuntu:~$ hostname
ubuntu

root@ubuntu:~$ hostname -I
172.30.1.2 172.17.0.1

root@ubuntu:~$ lscpu
Architecture:          x86_64
CPU(s):                1
Model name:            Intel Xeon E312xx (Sandy Bridge, IBRS update)
Hypervisor vendor:     KVM

root@ubuntu:~$ free -h
               total        used        free      shared  buff/cache   available
Mem:           1.9Gi       415Mi       871Mi       1.1Mi       783Mi       1.5Gi
Swap:          1.0Gi          0B       1.0Gi

root@ubuntu:~$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/vda1        19G  5.4G   13G  30% /
