---
title: Nmap Basics
date: 2023-01-23 18:15:41
tags: Enumeration
categories: infosec
links: https://bytexd.com/how-to-use-nmap/, https://www.geeksforgeeks.org/nmap-command-in-linux-with-examples/, https://infosecwriteups.com/a-beginners-guide-to-nmap-91aaecf15056, https://securitytrails.com/blog/nmap-commands
---

## What is Nmap?

Nmap (or “network mapper”) is one of the most popular free network discovery tools on the market. It allows the user to find live hosts on their network systems and scan for open ports and operating systems. When using Nmap scanning, the user simply enters commands and runs scripts via the text-driven interface. They can navigate through firewalls, routers, IP filters, and other systems. At its core, Nmap was designed for enterprise-scale networks and can scan through thousands of connected devices.

Some of the main uses include:

- Create a complete computer network map.
- Find remote IP addresses of any hosts.
- Get the OS system and software details.
- Detect open ports on local and remote systems.
- Audit server security standards.
- Find vulnerabilities on remote and local hosts.


The program works by using IP packets to identify available hosts on a network as well as what services and operating systems they run. Nmap is available on many different operating systems from Linux to Free BSD and Gentoo. 


## Instalation 

#### Install Nmap on MAC OS X

For Mac OS X you can check the installation instructions from Nmap.org to download and install the executable installer named nmap-<latest version>.dmg.

#### Install Nmap on Ubuntu and other Debian Based Distros

To install Nmap on Ubuntu and other Debian based distros, first we’ll update the package index.

``` bash
$ sudo apt-get update.
```
This way you will get the most updated versions of the package you are installing.

To install Nmap, run:

``` bash
$ sudo apt-get install nmap
```

After it’s done, open a command line and run the following command to check the Nmap version. This way we also know that Nmap is working.

``` bash
$ nmap --version
```


## How To Use Nmap?

Nmap is pretty easy to use if you're familiar with command-line interfaces. As it’s already installed on most Linux/Unix-based distributions, you just have to execute the ‘nmap’ command from any terminal, and that’s it. It will display several options for you. Advanced users will also be able to use Nmap along with other system scripts and automated tasks in order to maximize the powers of this tool.

Nmap port scan command

One of the most basic Nmap commands for a scan is the nmap port scan command:


``` bash
$ nmap -p 80 X.X.X.X
```
