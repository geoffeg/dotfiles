# geoffeg's dotfiles

A collection of my dotfiles. Based heavily on:

- [Marcel Patzwahl's](https://github.com/snowiow) [dotfiles](https://github.com/snowiow/snow) described in https://snow-dev.com/posts/next-level-dotfiles-with-ansible.html
- https://thebroken.link/managing-dotfiles-with-ansible/

## Installation

Clone the repo and run:

```
ansible-galaxy install -r requirements.yml
ansible-playbook -K dotfiles.yml
```

## License

MIT
