# Envs / MyDesktop Enviroment

## About the project
This project is a bunch of scripts to help me organize my work and studies on Machine learning, Deep Learning and DataScience.

It uses LXC/LXD as the core to initialize and launch containers that isolate DataScience libraries and environment from the Host. 
It's a working progress project where my goal is to let me very organized and efficient at my way to do things.

## Prerequisites
This scripts assumes the machine that will host it already have LXD REST API Server running. [source](https://github.com/lxc/lxd/) 

## The structure

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

## INSTRUCTIONS

1-Pre-Requesites (LXD/LXC) on the Host Machine

2-clone this source respository

3-copy /scripts/.env.bak to /scripts/.env

4-Fill the blanks on .env file

5-call the ./launch_gpu
