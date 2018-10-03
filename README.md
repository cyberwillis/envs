# Envs

## A word first
This project is just a bunch of scripts to help me organize the way I like to work in Machine learning and Deep Learning, it's not intended to be a software distribution or serves as incentive to anybody use the kind of software I like. It's just the way I like to do things.

## About
This project uses LXC/LXD as the core to launch and initialize containers to work with Data Science, Machine Learning and Deep Learning. This is also a working progress project where my goal is to be organized, learn more about the infrastruture of Containers, GPU on Containers and Local resources (Homemade Cloud).

## Prerequisites
This scripts and structure assumes the machine where it will be used already have LXC/LXD server containers running. Be it built by the used or installed via deb PPA or snapcraft. I will not give instructions to do so. But feel free to ask.

## The structure
In my day by day investigation and experimentation about Data Science and Machine Learning in General are based on this tools. I launch a container , inject the software I need on it or build inside of it and use it. I can make backups to later use or throw it away as I like. The same principles of Docker and LXC but the point is I use the way I intend not the way others want me to use. I don't care their best practices , my best practices are organized in my way of thinking and my way of customize things for my use and my needs. Not generic use. Anybody is welcome to look grab a copy use as they fit.

## Why
I started using docker to this matter but in less then a month I discovered that it was limited to my needs (create a environment to install many processes) and do Machine learning and Deep Learning using almost 100% of the Machine and GPUs. LXC doesn't rely on virtualize kernels , instead it uses the Kernel of the Bare Metal. It's like a Virtual Machine without a Kernel or a Container dependent of the Bare metal Kernel. 
It's ephemeral as you pleased to be and you can make clusters of it to work in parallel. Again, look outside to know more about LXC and its differenced of Docker. At first I started this organization project with docker but very after I realized that I need something more consistent so I started this project and depricated the earlier.

## INSTRUCTIONS
on scripts folder change the .env file to point to correct information that will be used by scripts

