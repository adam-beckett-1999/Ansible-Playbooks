![image info](ansible-playbooks.png)

---

## Ansible Playbooks for Home Network Management

This repository contains a collection of Ansible playbooks and roles for deploying and managing a home network environment. The playbooks cover a wide range of tasks, including virtualization, containerization, storage, monitoring, and general Linux system management.

> **Note:** This is a work-in-progress repository. Some playbooks/roles may be unfinished or have issues. Use at your own risk and adapt as needed for your environment.

---

### Playbooks

- `docker-prune.yaml` — Prune unused Docker images and containers
- `docker-server-stack-configure.yaml` — Configure Docker server stack
- `docker-swarm-server-stack-configure.yaml` — Configure Docker Swarm server stack
- `game-server-stack-configure.yaml` — Configure game server stack
- `kubernetes-cluster-stack-configure.yaml` — Configure Kubernetes cluster stack
- `lxc-containers-configure.yaml` — Configure LXC containers
- `patchman-install.yaml` — Install Patchman client
- `proxmox-update.yaml` — Update Proxmox servers
- `reboot.yaml` — Reboot target machines
- `shutdown.yaml` — Shutdown target machines
- `update-report-pve-clusters.yaml` — Generate update reports for Proxmox clusters
- `update-report-vms-lxcs.yaml` — Generate update reports for VMs and LXCs
- `vms-lxcs-update.yaml` — Update VMs and LXCs

---

### Roles

#### Proxmox Management
- `proxmox-create` — Create new Proxmox VMs
- `proxmox-clone` — Clone existing Proxmox VMs
- `proxmox-destroy` — Destroy Proxmox VMs
- `proxmox-snapshot` — Manage Proxmox VM snapshots
- `proxmox-vm-start` / `proxmox-vm-stop` — Start/stop VMs

#### Docker & Container Management
- `docker-install` — Install Docker
- `docker-image-prune` — Prune Docker images
- `docker-portainer-deploy` — Deploy Portainer
- `docker-portainer-agent-deploy` — Deploy Portainer Agent
- `docker-swarm-create` — Create Docker Swarm
- `docker-swarm-manager-join` / `docker-swarm-worker-join` — Join Swarm as manager/worker

#### Kubernetes & K3s
- `k3s-master-deploy` — Deploy K3s master
- `k3s-node-deploy` — Deploy K3s node
- `k3s-prerequisites` — Prepare system for K3s
- `kubernetes-portainer-agent-deploy` — Deploy Portainer Agent on Kubernetes

#### Storage & Network
- `glusterfs-configure` — Configure GlusterFS
- `glusterfs-mount` — Mount GlusterFS volumes
- `glusterfs-service` — Manage GlusterFS service
- `network-share-mount` — Mount network shares

#### System Management & Utilities
- `base-packages` — Install base packages
- `cc-amp-install` — Install AMP (Application Management Panel)
- `cockpit-install` — Install Cockpit web management
- `disable-motd-ubuntu` — Disable Ubuntu MOTD
- `patchman-client-install` — Install Patchman client
- `pause` — Pause execution
- `pufferpanel-install` — Install PufferPanel
- `qemu-guest-agent-install` — Install QEMU guest agent
- `reboot` / `shutdown` — Reboot or shutdown systems
- `reboot-required-check` — Check if reboot is required
- `snmp-configure` — Configure SNMP
- `update` — General update tasks
- `update-report-aggregated-alert` / `update-report-single-alert` — Update reporting
- `webmin-install` — Install Webmin

---

## Usage

Refer to individual playbooks and roles for usage details/required environment variables.

---
