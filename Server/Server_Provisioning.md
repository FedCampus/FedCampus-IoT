# Server Provisioning

## Layering structure
### Base Operating System (Type I hypervisor)

> To be decided, two choices below

- **[ProxmoxVE](https://www.proxmox.com/en/proxmox-ve)** with a free license is not production-ready but the management interface is better.

- **[ESXi](https://www.vmware.com/products/esxi-and-esx.html)** comes with a free license with every vmware account and is production-ready but it's management interface (WebUI) is not easy to navigate.

### Virtual Machines

#### Ubuntu Server 22.04.2 LTS (IoT Server)

- [Docker](https://docs.docker.com/engine/install/ubuntu/) host

    The containers are introduced [here](Server\_Structure.md).
- [Portainer](https://install.portainer.io/) for management of Docker Containers
- [Ansible](https://docs.ansible.com/) for all automated jobs

#### ML Server (OS TBD, GPU Passthrough)