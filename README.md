# Ansible-infra

## Synopsis

This repo helps provision a local infrastructure for Ansible playbooks development. Two Vagrant boxes on CentOS 7 are provisioned:
 - *ansible* - A control machine on 192.177.0.7
 - *develop1* - Target machine on 192.177.0.8

## Motivation

Ansible is currently not supported natively on Windows. This repo provides a development environment for ansible playbooks using Vagrant.

## Installation

Clone the repo and provision the machines with vagrant:
```
git clone https://github.com/mihail-dev/Ansible-infra.git
cd Ansible-infra
vagrant up
```
You can test Ansible with these commands
```
vagrant ssh
ansible --version
ansible develop1 -m ping
```
