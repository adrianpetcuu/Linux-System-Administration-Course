## Installing and Configuring a Clustered Environment on Linux

A clustered environment
consists of multiple Linux
systems working together
to provide high availability
and load balancing.

### Key Components
- Multiple nodes (servers)
- Shared storage (optional)
- Cluster communication network
- Cluster management software

### Common Cluster Tools
- Pacemaker – resource management
- Corosync – cluster communication
- pcs – cluster configuration tool

### Install Cluster Packages
```bash
dnf install pacemaker corosync pcs -y
```

### Enable and Start pcs Service
```bash
systemctl enable --now pcsd
```

### Set hacluster Password
```bash
passwd hacluster
```

### Authenticate Cluster Nodes
```bash
pcs host auth node1 node2
```

### Create Cluster
```bash
pcs cluster setup mycluster node1 node2
pcs cluster start --all
```

### Check Cluster Status
```bash
pcs status
```

### Summary
Linux clustering provides
high availability and fault
tolerance by allowing
multiple servers to act
as a single system.
