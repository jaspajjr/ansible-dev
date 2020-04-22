# Ansible Dev Env

## Getting Started

1. Ensure Ansible is installed, ideally from the Ansible repository or via pip (see [here](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html))
1. Clone this repository and ```cd``` to it

```bash
# To run it with default variables
ansible-playbook playbook.yml

# To see what it'll do
ansible-playbook playbook.yml --list-tasks --list-hosts

# To run it with custom values - recommended
ansible-playbook playbook.yml -e "user=JohnDoe dotfiles_src=https://github.com/JohnDoe/dotfiles.git"
```

## Troubleshooting

If Ansible complains about ```ansible.cfg``` being world-writable and therefore not a valid Ansible config, amend your permissions with chmod.

```bash
chmod 0755 //path/to/repo -R
```
