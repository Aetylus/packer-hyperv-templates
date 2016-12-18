# Packer Templates for Hyper-V

Packer configuration for creating Hyper-V Vagrant boxes.

Packer template and kickstart configuration based off [Bento](https://github.com/chef/bento).

## Requirements

* [Packer](https://www.packer.io/)
* Hyper-V

## Instructions

To build the packer template:

    $ packer build fedora-25.json

To add the box to vagrant:

    $ vagrant box add builds\fedora-25.hyperv.box --name NAME

where `NAME` is the name you want to give the box (i.e. `aetylus/fedora-25`).
