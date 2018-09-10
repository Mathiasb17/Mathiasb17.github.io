---
layout: post
title: "Build TokenPay GUI on Raspberry Pi"
comments: true
description: "Build the TokenPay GUI on your raspberry pi"
keywords: "TokenPay, Qt, GUI"
---

TokenPay is a cryptocurrency based on bitcoin's codebase, and based on a proof of stake (PoS) reward system.

Staking can be expensive because you need to have your wallet running 24/7. However, if you have a raspberry pi, the cost of staking decreases
dramatically. The power consumption of a raspberry pi 3b is about 0.005 kw/h which yearly costs about 7€ in France.

In this tutorial i'll assume you are running a Raspberry Pi 3 on raspbian.

### Step 1 : Increase the swap size

We first need to increase the swap size as the default value (100 MB) is too low to build the project and it will make your rpi crash.

Disable the swap : 

```
sudo dphys-swapfile swapoff
```

Then edit */etc/dphys-swapfile* with a text editor :

```
CONF_SWAPSIZE=1024
```

Finally enable the swap again :

```
sudo dphys-swapfile swapon
```
