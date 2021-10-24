# environments-docker-linux

How to use:
1. Copy or rename Dockerfile.example to Dockerfile
2. Change `ARG` values in the new Dockerfile
   - USER_PWD: Your default user password (eg: 123564)
   - USER_NAME: Your default username (eg: supersaian)
   - DOTFILES_REPO_URL: Your dotfiles repo url: (eg: https://github.com/akinozgen/environments)
   - DOTFILES_PATH: Dotfiles location in repository (eg: `/` or `/linux` in my case)
   - **Optionals**:
   - GITHUB_ACCESS_TOKEN: If you have a private dotfiles repo url set this to your access token. [Click to create new access token](https://github.com/settings/tokens/new)
   - SSH_PUBLIC_KEY_URL: If you got public/private key somewhere around the web, set this to its url
   - SSH_PRIVATE_KEY_URL: Same for SSH_PUBLIC_KEY_URL
   - SSH_KNOWN_HOSTS_FILE: Same for SSH_PUBLIC_KEY_URL
   - SHARED_FILESYSTEM_PATH: If you want to share a folder from your host computer, set this to a path that you want to mount.
