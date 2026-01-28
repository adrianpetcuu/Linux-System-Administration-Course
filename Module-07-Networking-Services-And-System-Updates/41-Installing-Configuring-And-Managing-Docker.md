## Installing, Configuring and Managing Docker

Docker is a popular
container platform used
to build, ship, and run
applications in containers.

### Install Docker
```bash
dnf install dnf-utils -y
dnf config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
dnf install docker-ce docker-ce-cli containerd.io -y
```

### Start and Enable Docker
```bash
systemctl enable --now docker
```

### Verify Installation
```bash
docker --version
docker run hello-world
```

### Manage Docker Service
```bash
systemctl status docker
systemctl restart docker
```

### Basic Docker Commands
```bash
docker ps
docker ps -a
docker images
docker pull nginx
```

### Run a Container
```bash
docker run -d -p 80:80 nginx
```

### Stop and Remove Containers
```bash
docker stop container_id
docker rm container_id
```

### Summary
Docker provides an
easy-to-use container
platform widely adopted
for application deployment
and development.
