---
title: "Mac"
date: 2021-02-21T12:37:54-05:00
draft: false
---


- `tmux -CC` to run a tmux session within iTerm2
    - `tmux -CC attach` to attach to an existing tmux session
- Prohibit sleep: `caffeinate` or with specified time `-t` in seconds
- Add spacer tile in doc: `defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock`