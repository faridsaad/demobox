Quick Demo Box
=================
Playbook to set up a demo box that allows terminal connection via HTTPS using ajaxterm.
 - It sets up the apache vhost as default-ssl. 
 - Basic htaccess username/password is enabled on vhost
 - Apache is configured to proxy connections over to ajaxterm.

Example use:
ansible-playbook -i hostlist -e 'htuser=testing htpass=faridtesting' main.yaml -vvv

Tested to work in Debian 8 and Ubuntu 16.04
