# Habitat build for ARM

## Configuration

* Raspberry Pi Zero W (ARMv6)
* Raspbian OS

## Instructions

Run everything as root.

```
$ sudo su -
```

Install Docker

```
$ curl -sSL https://get.docker.com | sh
```

Setup build environment variables

```
$ cat <<'EOF' > .build_env.sh
HAB_SCR_FOLDER="habitat"
HAB_VERSION="0.56.0"
HAB_ARTIFACTS="artifacts"
HAB_GIT="https://github.com/habitat-sh/habitat.git"
DOCKER_IMAGE="habitat-base:latest"
DOCKER_USER="build"
DOCKER_USER_PASS="password1"
DOCKER_USER_HOME="/home/build"
DOCKER_USER_SHELL="/bin/bash"
DOCKER_USER_SUDO_GRP="sudo"
EOF
```




