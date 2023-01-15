# macos-dev-setup

My personal guide and dotfiles for setting up a fresh install of MacOS for development.

## Steps

1. Get 1Password!

2. Download https://github.com/sufyan-motala/macos-dev-setup

3. Setup MacOS settings:

```bash
cd macos-dev-setup
./.macos
```

4. Get Homebrew:

```bash
sudo xcode-select --install
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
echo 'PATH="/usr/local/bin:$PATH"' >> ~/.zshrc
```

5. Check that Homebrew is installed correctly:

```bash
brew doctor
```

6. Install git

```bash
brew install git
```

7. Check git is installed correctly:

```bash
git --version
```

8. Install Python:

```bash
brew install python
pip install --upgrade setuptools
pip install --upgrade pip
```

9.  Install majority of apps with Homebrew:

```bash
cd macos-dev-setup
cat .brew | xargs brew install
```

10. Install remaining apps with App Store:
    
    1. 1Password extension
    2. Ledger Live
    3. Todoist
    4. VSCode
    5. Logi Options
    6. MS Office Suite + Teams
    7. etc.

11. Open iterm2 and install oh-my-zsh:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```