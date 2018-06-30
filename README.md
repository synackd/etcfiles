# synack.d's GNU/Linux System Configuration Files
This repository contains the system configuration files located in `/etc`, `/usr`, et
cetera which complement the dotfiles in my
[dotfiles](https://github.com/synackd/dotfiles) repository. Thus, the branches share the
names of those in that repository. So, just like it, each theme is located on its own
branch, with "daily driver" etcfiles located in `sandbox/<hostname>`. Enjoy!

## Requirements
* [Ansible](https://github.com/ansible/ansible)
    * This is only required if you want to automate the etcfiles installation. You can,
    of course, do it manually.

## Installation
To automatically install, use:
```bash
$ git clone https://github.com/synackd/etcfiles.git
$ git checkout <theme>
$ ansible-playbook -K ansible/main.yml
```

Where `<theme>` is the name of the branch where the desired theme resides.
You can also add the `--check --diff` options to see the differences between your
etcfiles and these without clobbering them.

Also, you can install certain dotfiles using Ansible tags by adding the
`--tags "<tag>"` option.
