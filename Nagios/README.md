Based off the installation guide: https://support.nagios.com/kb/article/nagios-core-installing-nagios-core-from-source-96.html

Some Vagrantfiles have also been provided that can be used to demonstrate the playbooks working.

A collection of playbooks:
  - play_setup_server.yml: Setups the Nagios Master Server.
  - play_setup_hosts.yml: Configures hosts and adds them to the Nagios Master Server.

The vars and secrets files follow this naming convention of "X_setup_[server|hosts].yml"

_vars_ is where user-set variables are. Stuff like `make_list`.
_secrets_ is where the `nagios_admin_pass` variable is; the vault password is 'password', as this is just for demonstration purposes.

TODO:
  - CentOS8/RHEL8 have a weird bug where even after nagios-core installation, the nagios.service doesn't exist
  - Get the playbook to add hosts to a Nagios Server working properly
  - Write a proper readme taht steps through how to execute and run all of this
