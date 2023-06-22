# Tailscale Deploy

Ansible playbook to deploy Tailscale with SSH and Exit Node enabled on 1 or more machines. This is a great way to self-host your own VPN, but keep it easy for all of your devices. Exit Nodes can easily be switched in the Tailscale apps.

> Supported operating systems:
> - Debian / Ubuntu
> - CentOS / RedHat
> - Rocky Linux / AlmaLinux
> - Amazon Linux 2023 / Amazon Linux 2
> - Fedora
> - Arch Linux
> - OpenSUSE
> - Oracle Linux
> - Raspbian
>
> From [ansible-role-tailscale](https://github.com/artis3n/ansible-role-tailscale)

# How to use

1. Clone this playbook with `git clone https://github.com/itsnebulalol/tailscale-deploy && cd tailscale-deploy`
2. [Install Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
3. Run `ansible-galaxy install -r requirements.yml --force`
4. Edit `hosts` with your server info, add as many servers as you need
5. Get a Tailscale auth key from [here](https://login.tailscale.com/admin/settings/keys)
6. Run the playbook with `TAILSCALE_KEY="key goes here" ansible-playbook -i hosts main.yml`

# Credits

- [Matrix Docker Ansible Deploy](https://github.com/spantaleev/matrix-docker-ansible-deploy) for `hosts` file and other references
- [artis3n](https://github.com/artis3n) for [ansible-role-tailscale](https://github.com/artis3n/ansible-role-tailscale)
