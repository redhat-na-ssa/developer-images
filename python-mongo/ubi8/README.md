# Developer Images

[![Build of UBI 8 based Developer Images](https://github.com/devfile/developer-images/actions/workflows/ubi8-build.yaml/badge.svg)](https://github.com/devfile/developer-images/actions/workflows/ubi8-build.yaml)

Containers images with tools for developers 👨‍💻👩‍💻

## Developer Base Image

### Red Hat Universal Base Image ([UBI](https://developers.redhat.com/articles/ubi-faq#)) based image ([quay.io/devfile/base-developer-image:ubi8-latest](https://quay.io/repository/devfile/base-developer-image))

Run the following command to test it with Docker:

```bash
$ docker run -ti --rm \
       quay.io/devfile/base-developer-image:ubi8-latest \
       bash
```
### Included Developement Tools

| Tool                | ubi8 based image                    |
|---------------------|-------------------------------------|
| `bash`              |`bash`                               |
| `bat`               |`<gh releases>`                      |
| `curl`              |`curl`                               |
| `ps`                |`ps`                                 |
| `diff`              |`diffutils`                          |
| `emacs`             |`NOT AVAILABLE (fedora only)`        |
| `fish`              |`NOT AVAILABLE (fedora only)`        |
| `gh`                |`<gh releases>`                      |
| `git`               |`git`                                |
| `git-lfs`           |`git-lfs`                            |
| `ip`                |`iproute`                            |
| `jq`                |`jq`                                 |
| `htop`              |`NOT AVAILABLE (fedora only)`        |
| `less`              |`less`                               |
| `lsof`              |`lsof`                               |
| `man`               |`man`                                |
| `nano`              |`nano`                               |
| `netcat`            |`NOT AVAILABLE`                      |
| `netstat`           |`net-tools`                          |
| `openssh-client`    |`openssh-clients`                    |
| `7z`                |`p7zip-plugins`                      |
| `ripgrep`           |`<gh releases>`                      |
| `rsync`             |`rsync`                              |
| `scp`               |`openssh-clients`                    |
| `screen`            |`NOT AVAILABLE`                      |
| `sed`               |`sed`                                |
| `shasum`            |`perl-Digest-SHA`                    |
| `socat`             |`socat`                              |
| `sudo`              |`sudo`                               |
| `ss`                |`NOT AVAILABLE`                      |
| `ssl-cert`          |`NOT AVAILABLE`                      |
| `tail`              |`<built in>`                         |
| `tar`               |`tar`                                |
| `time`              |`time`                               |
| `tldr`              |`NOT AVAILABLE (fedora only)`        |
| `tmux`              |`NOT AVAILABLE (fedora only)`        |
| `vim`               |`vim`                                |
| `wget`              |`wget`                               |
| `zip`               |`zip`                                |
| `zsh`               |`NOT AVAILABLE (fedora only)`        |
| **TOTAL SIZE**      | **412MB** (143MB compressed)        |

## Developer Python and MongoDB Image

### Red Hat Universal Base Image ([UBI](https://developers.redhat.com/articles/ubi-faq#)) based image ([quay.io/devfile/universal-developer-image:ubi8-latest](https://quay.io/repository/devfile/universal-developer-image))

Run the following command to test it with Docker: 

```bash
docker run -ti --rm \
       quay.io/redhat-na-ssa/python3-developer-image:ubi8-latest \
       bash
```
### Included Development Tools

| Tool or language    | ubi8 based image                    |
|---------------------|-------------------------------------|
|------PYTHON---------|-------------------------------------|
| `python`            |`python3.11`                         |
| `setuptools`        |`python3.11-setuptools`              |
| `pip`               |`python3.11-pip`                     |
| `pylint`            |`<via pip>`                          |
| `yq`                |`<via pip>`                          |
|--------MONGODB------|-------------------------------------|
| `mongosh`           |`2.2.6.x86_64`                       |
|------CLOUD----------|-------------------------------------|
| `oc`                |`mirror.openshift.com`               |
| `tkn`               |`mirror.openshift.com`               |
| `podman`            |`container-tools:rhel8`              |
| `buildah`           |`container-tools:rhel8`              |
| `skopeo`            |`container-tools:rhel8`              |
| `kubectl`           |`<kubernetes dnf repo>`              |
| `krew`              |`<gh releases>`                      |
| `helm`              |`<get.helm.sh>`                      |
| `kustomize`         |`<gh releases>`                      |
| `tkn`               |`<gh releases>`                      |
| `kn`                |`<gh releases>`                      |
| `terraform`         |`<releases.hashicorp.com>`           |
| `docker`            |`<download.docker.com>`              |
| `docker-compose`    |`<gh releases>`                      |
| `skaffold`          |`google releases`                    |
| **TOTAL SIZE**      | **3.75GB** (3.6GB compressed)       |

# Builds

This repo contains [actions](https://github.com/eclipse-che/che-operator/actions), including:
* [![release latest stable](https://github.com/devfile/developer-images/actions/workflows/ubi8-build.yaml/badge.svg)](https://github.com/devfile/developer-images/actions/workflows/ubi8-build.yaml)

# License

Che is open sourced under the Eclipse Public License 2.0.
