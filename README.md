# Old Chrome
This is an attempt to recreate the old chrome theme. [This](https://github.com/pratyushtewari/firefox-like-chrome) repository was used as a basis.

## Suggestions
- Set `browser.theme.dark-private-windows` to `false` in `about:config` tab (without this, the theme currently does not correctly display private mode)
- Set `browser.uidensity` to `1` (or any other value that suits you) `about:config` tab.

## Installation
- Go to `about:config` in a new tab and turn on the `toolkit.legacyUserProfileCustomizations.stylesheets` setting
- Type `about:profiles` in your address bar.
- Find the profile that is currently in use (usually next to it is written "This is the profile in use and it cannot be deleted.")
- Find the "Root Directory" entry in current profile and open it.
- Open or create a folder called "chrome" in the Root Directory. You might already have that folder with the userChrome.css there. You may want to back up this file. Just rename it to userChrome.css.bak
- Copy userChrome.css from this repository to this folder.
- Restart Firefox

## TODO's list:
- Carry out a complete refactoring of the code, thereby getting rid of the basis in the form of a third-party repository.
- Add support for dark private mode (currently `browser.theme.dark-private-windows` must be set to `false` in order for the theme to look acceptable)
- Get rid of hover selection on new tab button
- Get rid of the transparency of the hovered tab
- Fix new tab button position relative to tabs
