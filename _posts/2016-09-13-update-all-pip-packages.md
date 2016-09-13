---
layout: post
title: "Update All Python Pip Packages"
comments: true
description: "How to update all pip packages at once"
keywords: "python, pip"
---

#### Pip

Pip is the python package manager, pretty much like *npm* for node.

To update one package, one simply does :

```bash
sudo pip install --upgrade matplotlib
```
But one can't update them all at once directly with pip, so i did a small python program to do so :

```python
#!/usr/bin/python -O
import os
import re

print "Looking for outdated packages, this may take a while..."

outdated_packages = os.popen("pip list --outdated").read()

packages = outdated_packages.split('\n')

for pckg in packages:
	if(re.match("Could not find any downloads (.*)", pckg, re.M|re.I)): #nothing found on pip repositories for this package
		pckg_name = pckg.rsplit(None, 1)[-1]
		print "Cannot update "+pckg_name
	else:
		pckg_name = pckg.split(" ")[0]
		print "Updating " + pckg_name
		print os.popen("pip install --upgrade " + pckg_name).read()
```

Enjoy !
