# OpenBSD Basic Role 
Modify the base system just a tiny bit to make it a bit better looking and friendly.

This is made for personal use and is made so that it is as modular as possible.


## Role variables

| Variable | Default Value | Description |
| -------- | ------------- | ----------- |
| `base_ksh` | true | Very basic modification of default shell profile, loads all `*.sh` files in `/etc/profile.d/*.sh`. |
| `base_tmux` | true | Add a simple global `/etc/tmux.conf` tmux config, will be ignored if `~/.tmux.conf` exists. |
| `base_ssh` | true | Harden ssh to only pubkey login and only for `ssh-access` group. |
| `admin_user`| null | Needed if using `base_ssh` to allow atleast one user to login. |

For a detailed description of all variables look at the files [defaults/main.yml](defaults/main.yml) and [vars/main.yml](vars/main.yml).

