# Preferences
These settings and apps are optionnal and are anly a matter of taste, and work habits.

## Dock
To reduce the time used to display the dock when it is hide, run the following commands.
```bash
defaults write com.apple.dock autohide-delay -float 0      
defaults write com.apple.dock autohide-time-modifier -float 0.4; killall Dock
```

## Rectangle
It's a little app usefull for resizing and repositionning windows.
```bash
brew install --cask rectangle
```

## Fan Control
Mac Fans Control allows you to manage the power of your fans, it can be very usefull if you have some dust/crumb stuck in your fans, making an annoying noise.
```bash
brew install --cask macs-fan-control
```

## PDF compressor

Install this one with
```bash
brew install --cask pdf-squeezer
```