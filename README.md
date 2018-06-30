# synack.d's GNU/Linux System Configuration Files
This repository contains the system configuration files located in /etc, /usr, et cetera
which complement the dotfiles in my [dotfiles](https://github.com/synackd/dotfiles)
repository. Thus, the branches share the names of those in that repository. So, just
like it, each theme is located on its own branch, with "daily driver" etcfiles located
in `sandbox/<hostname>`. Enjoy!

## Installation
I have used [Ansible](https://github.com/ansible/ansible) to manage these files and
their installation. Thus, they can be installed with:
```bash
$ ansible-playbook -K ansible/main.yml
```
