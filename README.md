# Building a mini corporate network and configuring Active Directory

## Introduction

In this project, I build a mini corporate network setup and configured Microsoft Active Directory to perform basic administrative tasks.

![Visual](https://www.dropbox.com/scl/fi/xojfqtf8trm081fhxpkah/Active-Directory.png?rlkey=swe9k5yzgdy72s58vgsblq5x4&raw=1)

## What I did?

1. Setup a Windows 2019 on a Virtual Machine which plays the role of the Domain Controller.
2. Configured two Network Adapters on the Domain Controller: one for the outside internet, another one for the private network inside Virtualbox that the client should connect to.
3. Assigned manual IP address, subnet mask and DNS for the internal network. The external network get IP addressing from the home router.
4. Installed Active Directory and created a domain.
5. Configured NAT and Routing so that the client on the private network could reach the internet through the Domain Controller.
6. Setup a DHCP on the Domain Controller, so when a new client is created it could get automatically an IP address.
7. Created and ran a PowerShell script to automatically create a thousand users in Active Directory.
8. Created another Virtual Machine and installed Windows 10 on it. This VM is connected to the private Virtualbox network.
