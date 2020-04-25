---
title: '[Mosh for low-bandwidth ssh](https://mosh.org/#getting)'
collection: Links
tags:
  - Hacks
---
1. [Client side install if you are using Chrome](https://chrome.google.com/webstore/detail/mosh/ooiklbnjmhbcgemelgfhaeaocllobloj)
2. Server side insatll if you are using Ubuntu: `sudo apt-get install mosh`
3. Don't forget adding ssh key info
4. Kill past sessions except the existing one: `pgrep mosh-server | grep -v $(ps -o ppid --no-headers $$) && xargs kill || echo "no active sessions to kill"`