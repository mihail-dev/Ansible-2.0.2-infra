# Ansible-2.0.2-infra

## Synopsis

This repo helps provision a local infrastructure for Ansible playbooks development. Two Vagrant boxes on CentOS 7 are provisioned:
 - *ansible* - A control machine on 192.177.0.7
 - *develop1* - Target machine on 192.177.0.8

## Motivation

Ansible is currently not supported on Windows. 

## Installation

Clone the repo and provision the machines with vagrant:
```
git clone https://github.com/mihail-dev/Ansible-2.0.2-infra.git
cd Ansible-2.0.2-infra
vagrant up
```
You can test Ansible with these commands
```
ansible --version
ansible develop1 -m ping
```
