# DataBase Launcher

This Package installs followings:

- MySQL
- PostgreSQL
- MongoDB
- Adminer

## Setup Environment

### Step 1: Install Docker Engine

Use the following instructions to install the docker engine on Ubuntu, Debian and LinuxMint:

First, uninstall previous versions of Docker. Older versions of Docker were called docker, docker.io, or docker-engine. If these are installed, uninstall them:
```bash
$ sudo apt remove docker docker-engine docker.io containerd runc
```
It’s OK if `apt` reports that none of these packages are installed.

The contents of /var/lib/docker/, including images, containers, volumes, and networks, are preserved. The Docker Engine package is now called docker-ce.

Then, install docker using this command: 
```bash
$ curl -Ss https://get.docker.com | sudo bash
```
You can also use [official documentation of docker](https://docs.docker.com/engine/install/) to install docker engine on other platforms and operating systems.

### Step 1: Install Docker Compose

On Linux, these below step-by-step instructions are can help you to install Docker Compose:

First, run this command to download the current stable release of Docker Compose:

```bash
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.26.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
Finaly, apply executable permissions to the binary:

```bash
$ sudo chmod +x /usr/local/bin/docker-compose
```

For more information and install instructions for other operating systems take a look at [Docker Compose Official Documentation](https://docs.docker.com/compose/install/).

## Run Databases

After seting up environment, use below instructions to run databases and adminer:

First, clone this repo:
```bash
$ git clone https://github.com/farzad1120/my-dbs.git
```

Then, go into cloned folder:
```bash 
$ cd my-dbs
```

Finally, run docker compose up command:

```bash
$ docker-compose up
```
