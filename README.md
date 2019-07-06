## NetDevOps
#### 2019-07-06 claudia@indigowire.net

## Cosmic Cuttlefish Ansible In the Light (Documentation Version) Dockerfile
 - Latest Ubuntu LTS 18 Cosmic Cuttlefish
 	* 18.10, cosmic-20190131, cosmic, rolling (cosmic/Dockerfile)
 - Python 2.7, Python 3.6, Ansible 2.7, Nornir 2.0, Pandoc, Textlive
 - [Ansible 2.7 In the Light]( https://github.com/ansible/ansible/blob/stable-2.7/changelogs/CHANGELOG-v2.7.rst)
  

![Docker Icon](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSWmA-f2WW29z9uI8XXgshto0EjIOUqWwrRPBnpkaeQbOpFZRuW)

[cldeluna/cosmicd-light image](https://hub.docker.com/r/cldeluna/cosmic-lightd) 
  
------


Purpose built NetDevOps Ansible image starting with Ubuntu:18.10 Cosmic Cuttlefish base and including:
- Python 2.7 (Legacy)
- Python 3.6
- ansible 2.7
- git
- yaml
- jinja2
- tree
- nano
- vim
- wget
- traceroute
- iputils-ping
- snmp
- snmp-mibs-downloader
- pandoc
- texlive

Python Modules:
- nornir
- textfms
- netmiko
- ciscoconfparse
- argparse 
- requests
- xlrd
- openpyxl
- pandas

Repositories:
- https://github.com/cldeluna/ansible2_4_base.git
- https://github.com/cldeluna/cisco_aci.git
- https://github.com/cldeluna/cisco_ios.git


This is a larger version of the standard Docker Ansible container which includes enhanced support for generating documentation in Markdown and generation PDF files from MD files.


## Build

```
Claudias-iMac:cosmic-lightd claudia$ tree
.
├── AboutDocker.png
├── About_iMac.png
├── Dockerfile
└── README.md

0 directories, 4 files
```

```
Claudias-iMac:cosmic-light claudia$ docker build -t cldeluna/cosmic-light .
```

## Run

Run interactively and map a local directory /Users/claudia/Documents/docker_volume to the /ansible directory in the container.
```
Claudias-iMac:cosmic-light claudia$ docker run -v  /Users/claudia/Documents/docker_volume:/ansible -it cldeluna/cosmic-light
```

## Docker Hub

```
Claudias-iMac:cosmic-lightd claudia$ docker login
Claudias-iMac:cosmic-lightd claudia$ docker tag cldeluna/cosmic-lightd:latest cldeluna/cosmic-lightd:latest
Claudias-iMac:cosmic-lightd claudia$ docker push cldeluna/cosmic-lightd
```

## Environment

![About Docker](AboutDocker.png)

![About Docker](About_iMac.png)

