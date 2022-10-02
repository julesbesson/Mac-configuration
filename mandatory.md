# Mandatory installations on your Mac

This file explains

## HomeBrew

### Installation

Just run
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

To update (everything), run:
```bash
brew update
```

### wget

Please install `wget` by running:
```bash
brew install wget
```

## Git   
This allows to manage versions on your computer and online.

### Installation
To install Git, run:        
```bash
brew install git
```

### Configuration
Configure git with:
```bash
git config --global user.name "<GitHub-username>"
git config --global user.email <GitHub-email> 
```

### Get Git credential manager
Get it by running:
```bash
brew tap microsoft/git
brew install --cask git-credential-manager-core
```
you can update with
```bash
brew upgrade git-credential-manager-core
```

## Conda

### Installation

`conda` is a package manager, very useful to manage pyhton versions and packages. To install it, run:
```bash
brew install --cask miniforge
conda init zsh
```
Then restart your terminal.