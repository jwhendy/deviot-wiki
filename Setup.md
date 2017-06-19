# Deviot Setup

- [Python](#python)
- [Package Control](#package-control)
- [Manually](#manually)
- [Developer](#developer)

## Python
Before start to install Deviot make sure you have installed Python 2.x.

For windows you can download the installer from [this](https://www.python.org/downloads/) link. 

In UNIX environments python is already installed (in OS X since version 10.8)

## Package Control

To install Deviot from package control, first you need to install package control. If you already have installed, go to step 3

1. Go to [https://packagecontrol.io/installation](https://packagecontrol.io/installation) and copy the code in the grey box
2. Paste the code in the Sublime Text Console (`View > Console`) An input box will appear in the bottom of ST. When it finish to install will ask you to restart, in some cases more than one time.
3. Press `ctrl + shift + p` or go to `ST Menu > Preferences > Package Control` and select the option `Package Control: Install Package`. Write `Deviot` and waits until it's installed.

Deviot will show a window with the state of the installation.

## Manually

1. [Download](https://github.com/gepd/Deviot/archive/master.zip) Deviot from the master branch.
2. In Sublime Text go to `Preferences > Browse Packages...` and unzip the downloaded file there.
3. Restart Sublime Text and waits until the plugin is installed.

## Developer

To install the developer version go to `Preferences > Package Settings > Package Control > Settings - User` a new file will be open, paste:

```json
{
"repositories": ["https://github.com/gepd/Deviot/tree/develop"]
}
```

1. To upgrade the files open the Package Control quick panel `Preferences > Package Control` and select `Upgrade Package`. After some seconds the plugin will be updated.

2. If there is a new change in the branch and you are not receiving the update, select `Upgrade/Override All Packages` From the Package Control quick panel.