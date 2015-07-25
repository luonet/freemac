# Warning

此文档刚刚创建，目前极不完善，马上会修改出一个更好的版本，敬请关注。

# FreeMac

Build a free development environment on Mac OSX.

* Free, 是一种自由开放的心态。(Free mind, feel free)
* Free, 尽量使用免费软件（ 不一定是自由软件），尽量不使用盗版和破解软件。
* Free, 原作者来自 FreeWheel.

## Table of Contents

* [Principles](#principles)
* [System Preferences](#system-preferences)
  * [System Language](#system-language)
  * [Keyboard](#keyboard)
  * [Trackpad](#trackpad)
  * [Dock](#Dock)
  * [Spotlight](#Spotlight)
  * [输入法](#输入法)
  * [Mission Control](#mission-control)
* [Tools](#tools)
  * [Automatic Installation](#automatic-installation)
  * [Homebrew](#homebrew)
  * [Homebrew Cask](#homebrew-cask)
  * [iTerm2](#iterm2)
  * [Zsh](#zsh)
  * [Vim](#vim)
  * [Tmux](#tmux)
  * [Vagrant](#vagrant)
  * [Browser](#browser)
  * [科学上网](#科学上网)
* [快捷键](#快捷键)
* [Tips](#tips)
* [References](#references)

## Principles

1. 目标：Productive & Efficient. 不要玩物丧志。
2. 深思熟虑。自动化。KISS.
3. 谦卑。闻道有先后，taste 没什么了不起的。

## System Preferences

System Preferences may need your manual operations.

### System Language

#### What

English is preferred.

#### Why

More friendly to developers, easier to communicate, more resources when you searching internet.

#### How

1. Open System Preferences.
2. Choose View > Language & Region or click the Language & Region icon.
3. In the Languages pane, drag your preferred language to the top of the list. If you don't see your language, click the Add Language (+) button.
4. To apply the language throughout your system, restart your Mac, or log out and log back in.

#### Reference

* https://support.apple.com/en-us/HT201726

### Keyboard

#### Why

You can even bear the default keystroke speed? Seriously, as a programmer?

#### How

1. Open *System Preferences |> Keyboard*.
2. Change *Key Repeat* to *Fast*, change *Delay Until Repeat* to *Short*.

### Trackpad

1. Check *Tap to click*.
2. Check *Three finger drag* (This option in new forcetouch Macbook is hidden in *Accessiblity |> Mouse & Trackpad |> Trackpad Options |> Enable dragging*).

### Dock

#### Why

Get more spaces from dock.

#### How

1. Change position to left.
2. Check *Automatically hide and show the dock*.
3. Remove uncommon used applications from dock.

### Spotlight

1. Uncheck fonts, images, files etc.
2. 推荐快捷键使用 CMD+SPACE, 与输入法对调。

### 输入法

##### What

1. 推荐使用百度或搜狗输入法。我目前使用百度。
2. 同步词库与个人配置。
3. Keyboard |> Input Sources |> Automatically switch

### Mission Control

使用 HotCorners 快速关闭屏幕。

## Tools

### Automatic Installation

```
sh -c "`curl -fsSL https://raw.githubusercontent.com/luonet/freemac/master/install`"
```

### XCode

通过 App Store 安装完整版或通过命令行安装：

```
xcode-select --install
```

### Homebrew

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### Homebrew Cask

```
brew install caskroom/cask/brew-cask
```

### iTerm2

```
brew cask install iterm2
```

### Zsh

```
brew install zsh
```

`chsh -s /bin/zsh` or `chsh -s /bin/local/zsh`

### Oh My Zsh

```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Vim

[luonet's vim automatic installation](https://github.com/luonet/dotfiles):

```
sh -c "`curl -fsSL https://raw.githubusercontent.com/luonet/dotfiles/master/install`"
```

### Tmux

```
brew install tmux
```

### Quicklook

```
brew cask install qlmarkdown betterzipql webpquicklook qlcolorcode
defaults write com.apple.finder QLEnableTextSelection -bool TRUE;killall Finder
```

### Vagrant

```
brew cask install vagrant virtualbox
```

### Finder Enhancement

```
brew cask install xtrafinder
brew cask install go2shell
```

### Browser

```
brew cask install firefox
```

### Evernote

```
brew cask install evernote
```

### Video Player

```
brew cask install mplayerx
brew cask install vlc
```

### Screen Recorder

```
brew cask install licecap
brew cask install keycastr
```

### Others

```
brew cask install the-unarchiver
brew cask install spectacle
brew cask install cheatsheet
brew cask install appcleaner
```

### 科学上网

```
brew cask install shadowsocksx
```

If you are using OpenVPN:

```
brew cask install tunnelblick
```

## 快捷键

## Tips

## References

* http://sourabhbajaj.com/mac-setup/
* https://github.com/thoughtbot/laptop https://raw.githubusercontent.com/thoughtbot/laptop/master/mac
* https://gist.github.com/visioncan/7a1762196f80298fc377
* https://github.com/sindresorhus/quick-look-plugins
