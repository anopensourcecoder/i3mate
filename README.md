# i3-mate

Ansible playbook to install and configure i3 on Ubuntu Mate.

This playbook installs i3 and more.

## Features

This Ansible role installs the following components:

  * [i3](https://i3wm.org/) the tiling window manager.

## Usage

First install ubuntu mate ( Offline for faster installation)
Install vmware-tools if you are using VMware ( Skip on real machine )
Login and Disable automatic updates ( To avoid update nag inside vm)
Set the the main repo to nearby ( Helps with faster update)
Open terminal and run
    sudo apt install git
    sudo apt install ansible

    ```
    cd ~/Downloads/
    git clone https://github.com/anopensourcecoder/i3mate.git
    cd i3mate
    cp vars/vars.yml.example vars/vars.yml
    nano vars/vars.yml #update with your username and your password.
    ```

Then you can start the playbook:

    ```
    ansible-playbook playbook.yml -i hosts -e action=install
    ```

 ## TODO
  * Use existing mate utilities.
