# Envs

## A word first
This project is just a bunch of scripts to help me organize my work on Machine learning and Deep Learning using container as a Desktop,

## About
This project uses LXC/LXD as the core to launch and initialize containers to work with Data Science, Machine Learning and Deep Learning. 
This is also a working progress project where my goal is get my stuff organized, while I learn about Data Science Machine Learning and Deep Learning, Cloud Computing Infrastruture whith Containers (IaaS).

## Prerequisites
This scripts assumes the machine that will host it already have LXD/LXC REST API Server running.
Normally it's can be installed Ubuntu/Debian related machines using Lastest Distros or using Snapcraft on Ubuntu, or even building from the [source](https://github.com/lxc/lxd/) 

## The structure
In my day by day in Data Science and Artificial Intelligence I launch a container, inject the software I need on it (installing or building from source) and use it.

```
envs
│
├── backups
│   └── (*just containers and image backups here*)
├── frameworks
│   └── (*just libraries and frameworks that need to be built*)
├── projects
│   └── (*many folders of projects involving DS/ML/DL*)
├── repository
│   └── nvidia-repository-local
│        └── (*offline files of cuda tookit to fastest setup*)
├── scripts
│   └── (*bunch of shell scripts to launch and build my LXD containers*)
├── shared
│   └── (*folder shared beetwen the HOST and all the GUESTs*)
└── utils
    └── (*installer files that I may need in any GUEST*)
```


## Why
I started using docker in 2016 but I had the ideia do build containers to learn Machine Learning more easly in middle 2017, as the time passed I saw the comunity changing a lot so I started to notice latency on docker and the scenario changing, that made me think a new approach to virtualize GPU on container when I finally found LXD/LXC and started to launch container and run Machine Learning algorithms inside of it and totally like a Cloud Experience and also isolated from my own files in my Host machine.

## INSTRUCTIONS

1-Pre-Requesites (LXD/LXC) on the Host Machine
2-clone this source
3-copy /scripts/.env.bak to /scripts/.env
4-on that .env file fill the blanks of your location of this structure on your SSD/HDD Disk, configuring the compute capability for you GPU and the Jupyter secret password
5-execute the command ./launch_gpu


