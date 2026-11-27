# web_server

Setting up a web server with nginx and a domain name.

## Files

| File | Description |
| --- | --- |
| `0-transfer_file` | Transfers a file to a server with `scp` (takes file path, IP, username, and key path) |
| `1-install_nginx_web_server` | Installs nginx and serves a page containing `Holberton School` |
| `2-setup_a_domain_name` | The domain name pointing to the web-01 server |
| `3-redirection` | Configures nginx with a 301 redirection for `/redirect_me` |
| `4-not_found_page_404` | Adds a custom 404 page containing `Ceci n'est pas une page` |
| `5-design_a_beautiful_404_page.html` | A designed 404 page |

## Usage

```
./0-transfer_file PATH_TO_FILE IP USERNAME PATH_TO_SSH_KEY
```

The nginx scripts are run on the server itself as root:

```
sudo ./1-install_nginx_web_server
```

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All files end with a new line
- All Bash scripts are executable, start with `#!/usr/bin/env bash`, and
  have a comment on the second line explaining what the script does
- `systemctl` is not used to restart nginx
