# Default Setup for Ubuntu NGINX MySQL On Vagrant

This project automates the setup of a LEMP development environment.

## Requirements

* [VirtualBox](https://www.virtualbox.org)

* [Vagrant](http://vagrantup.com)

* [Cygwin](https://www.cygwin.com/) or any other ssh-capable terminal shell for the `vagrant ssh` command

## Recommended Workflow

The recommended workflow is

* edit files in the host computer

* run within the virtual machine

Your home folder is synced to `/home/vagrant/code` on the guest.

## Database
* For mysql the default user is root: `mysql -u root`


## Virtual Machine Management

When done just log out with and suspend the virtual machine

    host $ vagrant suspend

then, resume to hack again

    host $ vagrant resume

Run

    host $ vagrant halt

to shutdown the virtual machine, and

    host $ vagrant up

to boot it again.

You can find out the state of a virtual machine anytime by invoking

    host $ vagrant status

Finally, to completely wipe the virtual machine from the disk **destroying all its contents**:

    host $ vagrant destroy # DANGER: all is gone

Please check the [Vagrant documentation](http://docs.vagrantup.com/v2/) for more information on Vagrant.