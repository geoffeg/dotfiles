# geoffeg's dotfiles

A collection of dotfiles. Can be installed manually, or via ansible using [Jeff Geerling's](https://www.jeffgeerling.com/) [dotfiles ansible role](https://galaxy.ansible.com/geerlingguy/dotfiles/). 

If you've cloned this repo and have [ansible installed](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html), you can run:
```
ansible-galaxy install -r requirements.txt && ansible-playbook -e 'dotfiles_repo: https://github.com/geoffeg/dotfiles' -e 'dotfiles_repo_local_destination: ~/src/dotfiles' -i 'locahost,' dotfiles.yml
```

If you'd like to invoke the ansible role directly, without first cloning this repo:
```
ansible-galaxy install geerlingguy.dotfiles && ansible-role -e 'dotfiles_repo: https://github.com/geoffeg/dotfiles' -e 'dotfiles_repo_local_destination: ~/src/dotfiles' -i 'localhost,' --hosts localhost geerlingguy.dotfiles
```

## License

MIT
