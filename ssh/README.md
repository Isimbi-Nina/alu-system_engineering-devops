# alu-system_engineering-devops

System engineering and DevOps projects.

## 0x0B. SSH

Learning how to connect to a remote server securely with SSH, using key
pairs instead of passwords.

### Requirements

- Ubuntu 20.04 LTS
- Allowed editors: `vi`, `vim`, `emacs`
- All files end with a new line
- All Bash scripts are executable, start with `#!/usr/bin/env bash`, and
  have a comment on the second line explaining what the script does

### Files (`ssh/`)

| File | Description |
| --- | --- |
| `0-use_a_private_key` | Bash script that connects to the server as `ubuntu` using the private key `~/.ssh/school` |
| `1-create_ssh_key_pair` | Bash script that creates a 4096-bit RSA key pair named `school`, protected by a passphrase |
| `2-ssh_config` | SSH client configuration that uses `~/.ssh/school` and refuses password authentication |

Task 3 (adding a public key to the server) is done directly on the server
in `~/.ssh/authorized_keys`, so it has no file in this repo.

### Usage

```
./1-create_ssh_key_pair
./0-use_a_private_key
```

### Notes

The private key (`school`) is never committed to this repository.
