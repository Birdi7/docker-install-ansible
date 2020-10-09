# For what?
Installs docker & docker-compose on Ubuntu server via ssh.

# How to use?
1. Add your ssh key on your server;
2. Install on the server ansible: `brew install ansible`;
3. Change in [provisioning/hosts.yml](provisioning/hosts.yml) variable `ansible_host` on your server's indicator;
4. Run `ansible-playbook provisioning/site.yml -i provisioning/hosts.yml`;
5. Joy!

# In case when something does not work
1. Check `sudo systemctl status docker`. If status is dead - `sudo systemctl run docker`.
