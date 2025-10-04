# https://docs.astronvim.com/mappings

# 1. install nvim

```
  curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
  sudo rm -rf /opt/nvim-linux-x86_64
  sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz
```

#Then add this to your shell config (~/.bashrc, ~/.zshrc, ...):

```
  export PATH="$PATH:/opt/nvim-linux-x86_64/bin"
```

# 2. install tree-sitter

```
  npm install tree-sitter-cli
```

# 3. install ripgrep

```
  sudo apt-get install ripgrep
```

#4. install lazygit

```
  LAZYGIT*VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | \grep -Po '"tag_name": *"v\K[^"]*')
  curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/download/v${LAZYGIT_VERSION}/lazygit*${LAZYGIT_VERSION}\_Linux_x86_64.tar.gz"
  tar xf lazygit.tar.gz lazygit
  sudo install lazygit -D -t /usr/local/bin/
```

# 5. install go DiskUsage()

```
  sudo apt-get install gdu
```
