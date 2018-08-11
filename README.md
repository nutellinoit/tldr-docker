# TLDR docker image

Automatic build of https://github.com/tldr-pages/tldr

Add alias on `~/.bashrc` or `~/.zshrc`: `alias tldr='docker run --rm -it -v ~/.tldr/:/root/.tldr/ nutellinoit/tldr'`

Use `tldr` command