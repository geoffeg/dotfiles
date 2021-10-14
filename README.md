# geoffeg's dotfiles

A collection of my dotfiles. Based heavily on:

- [Marcel Patzwahl's](https://github.com/snowiow) [dotfiles](https://github.com/snowiow/snow) described in https://snow-dev.com/posts/next-level-dotfiles-with-ansible.html
- https://thebroken.link/managing-dotfiles-with-ansible/

This repo contains an [Ansible](https://docs.ansible.com/ansible/latest/index.html) playbook that installs a base set of utilities and, if available, their configuration files, via a set of Ansible roles.

## Installation

[Install Ansible](https://docs.ansible.com/ansible/latest/installation_guide/index.html), clone this repo and run:

```
ansible-galaxy install -r requirements.yml
ansible-playbook -K dotfiles.yml
```

## License

MIT
