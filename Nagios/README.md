## Ansible Playbook: Nagios Installation

Based off the installation guide: https://support.nagios.com/kb/article/nagios-core-installing-nagios-core-from-source-96.html

Will install Nagios-Core onto an Ubuntu2004 VM. I used Vagrant to create the VM, and the Vagrantfile has been provided, however the aim is that this is translatable to real-life systems. This should hopefully also apply to Ubuntu 2104.  

_vars.yml_ is where user-set variables are. Stuff like `make_list`.

_secret.yml_ is where the `nagios_admin_pass` variable is; the vault password is 'password'. This is just to demonstrate the use of Ansible-Vault within this playbook.

### Future Enhancements

- [] Extend to ensure this works with RHEL8
- [] Extend to include installation of the Nagios plugins
