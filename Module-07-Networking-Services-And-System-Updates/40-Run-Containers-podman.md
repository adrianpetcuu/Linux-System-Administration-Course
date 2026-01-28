## Run Containers (Podman)

Podman is a container
management tool used
to run and manage
containers without
a daemon.

### Key Features
- Daemonless container engine
- Compatible with Docker CLI
- Rootless containers supported
- Default container tool on RHEL/CentOS

### Install Podman
```bash
dnf install podman -y
```

### Run a Container
```bash
podman run hello-world
```

### Run Interactive Container
```bash
podman run -it ubuntu /bin/bash
```

### List Containers
```bash
podman ps
podman ps -a
```

### List Images
```bash
podman images
```

### Stop and Remove Container
```bash
podman stop container_id
podman rm container_id
```

### Pull Container Image
```bash
podman pull nginx
```

### Summary
Podman allows secure
and efficient container
management without
requiring a background
daemon.
