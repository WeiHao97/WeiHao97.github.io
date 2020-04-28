---
title: 'Login to Jupyter Notebook remotely'
collection: Links
tags:
  - Hacks
---
1. On server: `jupyter notebook --no-browser --port=8889`
2. On local terminal: `ssh -N -f -L localhost:8888:localhost:8889 username@serverIP`
3. On local browser: Open http://localhost:8888/ with token