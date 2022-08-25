---

layout: post
title: macOS Setup
categories: Tool
description: Tool
keywords: macOS,Tool

---

# System Preferences
Dock  
在 `System Preference > Dock & Menu Bar` 里，把 `Show recent applications in Dock` 前面的勾去掉。  
```
defaults write com.apple.dock persistent-apps -array; killall Dock
```

# Apps
CleanMyMac  

# References
[https://github.com/xiaolai/apple-computer-literacy](https://github.com/xiaolai/apple-computer-literacy)  

# brew
brew install todo  