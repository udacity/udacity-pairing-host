[![Build Status](https://travis-ci.org/udacity/udacity-pairing-host.svg?branch=master)](https://travis-ci.org/udacity/udacity-pairing-host)

# udacity-pairing-host

Is ...

  - An ansible role to initialize a host for remote pairing
  - An [ansible-pull] compatible playbook for standalone installations.

## version

1.0

## requirements
- for ansible-pull, ansible must be installed

## role variables

## standalone

The `local.yml` play uses the role to install the tools locally, either via manual execution or [ansible-pull].

```bash
# installs role locally
git clone git@github.com:udacity/udacity-pairing-host.git
cd udacity-pairing-host
ansible-playbook -i /dev/null local.yml

# ... or use ansible-pull
ansible-pull -U git@github.com:udacity/udacity-pairing-host.git
```

## wemux/tmux
### keybindings
todo

## license
Source Copyright © 2015 Udacity. Distributed under the GNU General Public License v3, the same as Ansible uses. See the file COPYING.
