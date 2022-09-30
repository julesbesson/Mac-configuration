# Code editors

To write, modify or execute programms, you need to have software that allow it. Here is a list of all the editors I use.

## Visual Studio Code
The most versatile one. It can manage almost every language, and is very useful to modify multi-languages projects.

### Installation
To install it:
```bash
brew install --cask visual-studio-code
```
Then
1. Open **VS-Code**.
2. Open *command palette* by pressing <kbd style = "large">F1</kbd> or <kbd style = "font-size:Large">⌘</kbd> + <kbd style = "font-size:Large">⇧</kbd> + <kbd style = "font-size:big">P</kbd>.
3. Type `Shell` in *command palette*.
4. Select `Shell Command: Install code in PATH` from suggested list.

Now, whenever you type `code .` in a folder, it will open it in **VS-Code**.

### Extensions
Here is the list of extensions I use.
- `Jupyter`
- `Python`
- `Markdown Preview Github Styling`
- `LaTeX Workshop`
- `PHP Intelephense`
- `French Laguage Pack For Visual Code`
- `HTML CSS Support`

## Pyzo
Pyzo is my favourite python IDE, easy to use and parameter.

### Installation
Just run
```bash
brew install --cask pyzo
```

### Setup
You can configurate Shells, which is very usefull. To do so, press <kbd style = "font-size:Large">⌘</kbd> + <kbd>,</kbd> to open preferences, and create 4 shells, one for each python environnment. You can name them `Python`, `Math`, `App` and `Sage`.

For the `Sage` shell, check "code à exécuter au démarrage" and then in *startupScript*, type
```python
# AFTER_GUI - code below runs after integrating the GUI
from sage.all import *
```

## Texmaker

It is an editor for LaTeX, my favourite on Mac. To install it, run
```bash
brew install --cask texmaker
```