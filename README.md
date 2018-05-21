# cookiecutter-ansible-vagrant

[Cookiecutter](https://github.com/audreyr/cookiecutter) template for a plain [Vagrant](https://www.vagrantup.com/) VM
provisioning using [Ansible](https://www.ansible.com/).

This is meant to be a simple Cookiecutter template on which a proper Ansible provisioning which is testable on a Vagrant
instance can be built. As such, the initial template makes some opinionated decisions, such as:

  * Only supporting [VirtualBox](https://www.virtualbox.org/) as the Vagrant VM provider.
  * Disabling folder sync in the Vagrant VM.
  * Disabling strict host key checking in Ansible's SSH connection.

You are of course free to modify these values after the template is instantiated. It's only that these options are not
(and will probably never be) exposed as Cookiecutter configurations.


# Usage

Read more about using [Cookiecutter](https://cookiecutter.readthedocs.io/en/latest/usage.html). This template in
particular was written using Cookiecutter v1.5.1 on Python 3.6.

Other versions of Cookiecutter and/or Python may work, but they have not been explicitly tested.

After instantiating the template, you can start using Vagrant to spawn the VM and provision it:

  $ vagrant up
