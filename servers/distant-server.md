# Distant servers

If you have to manage files in a distant folder, you can do it by two means.

## With terminal
It's a bit trickier, but you should manage to do it without big difficulties. The big downside is the lack of visibility.

### Connexion

```bash
ssh login@url
```
Then type your password and manage your files with `cd`, `mkdir`, `rm` ...

## Woth Forklift
It's an app that manages distant files and folder with a classic interface. 

### Installation
```bash
brew install --cask forklift
```

### Connexion

Open you app, then press <kbd style = "font-size:Large">⌘</kbd> + <kbd>K</kbd>. You now have to fill in the fields by the following way:
Field | Filling
:---: | :---:
`Protocol` | SFTP
`Server` | url
`Username` | login
`Password` | Password

## Webpage ENS Rennes

I advice to have a git repository which contains all the files of your page with link "git-web-url", then run
```bash
ssh login@ssh.eleves.ens-rennes.fr
```
Type your password, then run
```bash
git clone url public_html
```

To update it, simply update your git repository then connect to the server via terminal, and run
```bash
cd public_html
git pull
```
