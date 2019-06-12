# Dotfiles

This repository is an attempt to collect scripts together to make my entire (MacOS) system entirely reproducable.
See Mina Markham's setup for details

## ITerm2
Dotfiles created following (this blog post)[stratus3d.com/blog/2015/02/28/sync-iterm2-profile-with-dotfiles-repository/]

To Restore settings, check the “Load preferences from folder” option in Preferences and navigate to the file that already exists inside your dotfile repository.

You actually don’t have to use the iTerm2 GUI to load the preferences. It’s possible load them from the command line. This makes it easy to load them from a setup script in your dotfile repository. All you need are these two commands:

```
# Specify the preferences directory
defaults write com.googlecode.iterm2.plist PrefsCustomFolder -string "~/.dotfiles/iTerm2"
# Tell iTerm2 to use the custom preferences in the directory
defaults write com.googlecode.iterm2.plist LoadPrefsFromCustomFolder -bool true
```

## VSCode 
Dotfiles created following (this blog post)[https://pawelgrzybek.com/sync-vscode-settings-and-snippets-via-dotfiles-on-github/]

Extensions and other settings uploaded via (this extension)[https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync]
To download your settings, first install (this extension)[https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync] and then use the github token and gist ID

