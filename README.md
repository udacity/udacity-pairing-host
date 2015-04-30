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
ansible-pull --accept-host-key -o -U https://github.com/udacity/udacity-pairing-host.git
```

## wemux/tmux

### Creating/Joining sessions
[Wemux Host and Client Commands](https://github.com/zolrath/wemux#host-commands)

### keybindings
| description | key
------------- | ---
view key bindings | `C-a ?` ("q" to quit)
detach from session (leaves it running) | `C-a d` or `C-a C-d`
create window | `C-a c`
previous window | `C-a p` or `C-a C-p`
next window | `C-a n` or `C-a C-n`
select window # | `C-a #` (where # is 0-9)
scrollback (copy) mode | `C-a ESC` ("q" to quit)

## license
Source Copyright © 2015 Udacity. Distributed under the GNU General Public License v3, the same as Ansible uses. See the file COPYING.
