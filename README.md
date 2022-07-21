> Simple script to auto-init a Linux system

## Setup - Vars

- `cp .env-sample.yml .env.yml`
- Set the `user` variable.
- Set the `ssh_passphrase` variable (or leave blank for a less secure setup).

## Run

Install `ansible` and run:

```shell
ansible-playbook run.yml --extra-vars=@.env.yml --ask-become-pass
```
