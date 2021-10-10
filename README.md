# geoffeg's dotfiles

A collection of dotfiles. Can be installed manually, or via ansible using [Jeff Geerling's](https://www.jeffgeerling.com/) [dotfiles ansible role](https://galaxy.ansible.com/geerlingguy/dotfiles/). 

## Installation

Clone the repo, preferably into the same directory you'll set the roles `dotfiles_repo_local_destination` to:
```
mkdir -p ~/src/ && git clone https://github.com/geoffeg/dotfiles.git ~/src/dotfiles
```

Install the requirements and run the playbook:
```
ansible-galaxy install -r ~/src/dotfiles/requirements.yml && ansible-playbook -e 'dotfiles_repo: https://github.com/geoffeg/dotfiles' -e 'dotfiles_repo_local_destination: ~/src/dotfiles' -i 'localhost,' ~/src/dotfiles/dotfiles.yml
```

## License

MIT
