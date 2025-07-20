# Ansible Playbooks

![image info](ansible-playbooks.png)

---

## Ansible Playbooks for Home Network Management

This repository contains a collection of Ansible playbooks and roles for deploying and managing my homelab network environment. The playbooks cover a wide range of tasks, including virtualization, containerization, storage, monitoring, and general Linux/Windows system management.

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

- `docker-install` — Install Docker Engine
- `docker-image-prune` — Prune unused Docker images
- `docker-portainer-deploy` — Deploy Portainer management interface
- `docker-portainer-agent-deploy` — Deploy Portainer Agent
- `docker-swarm-create` — Initialize Docker Swarm cluster
- `docker-swarm-manager-join` — Join nodes to Swarm as managers
- `docker-swarm-worker-join` — Join nodes to Swarm as workers

#### Kubernetes & K3s

- `k3s-master-deploy` — Deploy K3s master node
- `k3s-node-deploy` — Deploy K3s worker node
- `k3s-prerequisites` — Prepare system for K3s installation
- `kubernetes-portainer-agent-deploy` — Deploy Portainer Agent on Kubernetes

#### Storage & Network

- `glusterfs-configure` — Configure GlusterFS distributed storage
- `glusterfs-mount` — Mount GlusterFS volumes
- `glusterfs-service` — Manage GlusterFS service
- `network-share-mount` — Mount network shares (SMB/NFS)

#### System Management & Utilities

- `base-packages` — Install essential base packages
- `cc-amp-install` — Install AMP (Application Management Panel)
- `cockpit-install` — Install Cockpit web-based management
- `disable-motd-ubuntu` — Disable Ubuntu MOTD messages
- `patchman-client-install` — Install Patchman patch management client
- `pause` — Pause playbook execution
- `pufferpanel-install` — Install PufferPanel game server management
- `qemu-guest-agent-install` — Install QEMU guest agent for VMs
- `reboot` — Reboot target systems
- `shutdown` — Shutdown target systems
- `reboot-required-check` — Check if system reboot is required (Linux/Windows)
- `snmp-configure` — Configure SNMP monitoring
- `update` — Perform system updates (Linux/Windows)
- `update-report-aggregated-alert` — Send aggregated update reports
- `update-report-single-alert` — Send individual update reports
- `webmin-install` — Install Webmin web administration

---

## License

This project is provided as-is for educational and personal use. Adapt and modify as needed for your environment.

---
