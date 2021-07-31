---
author: "Reperak"
date: "2021-07-31"
tags: ["monero", "xmrig"]
title: "Maximizing Your Monero Mining Profits"
---

## Introduction
Looking to maximize your Monero mining profits? This guide will show you how to increase your earnings using the Zorroware XMRig fork and MoneroOcean's algorithm switching.

## Setting up Zorroware's XMRig fork
Using Linux is recommended, as many of Zorroware XMRig's performance advantages are not available on other platforms.

Support for our fork will not be guaranteed from the XMRig developers or MoneroOcean.

### Downloading
Clone the Git repository using the following command, or [download it as a ZIP](https://github.com/zorroware/xmrig-zw/archive/refs/heads/master.zip).
```bash
git clone https://github.com/zorroware/xmrig-zw.git --depth=1
```

### Compiling
#### Windows
If you're building on Windows, follow the instructions [here](https://xmrig.com/docs/miner/build/windows).

Note that many of Zorroware XMRig's features will be missing, such as the Clang compiler and auto-compiling libraries.

#### Linux
If you're building on Linux, you will need to install a minimum of the dependencies listed in the "Advanced Build" section of the [XMRig build documentation](https://xmrig.com/docs/miner/build) for your distribution.

After the dependencies are installed, it's literally as simple as executing one of the shell scripts we've made.

If you want a full XMRig suite, run `./full_build.sh`

If you want an XMRig binary for plain old CPU mining, run `./lite_build.sh` (recommended)

If all goes well, you should have an XMRig binary in the build directory.

### Setting up the miner
Download a copy of [our config template](https://raw.githubusercontent.com/zorroware/xmrig-zw/master/src/config.json) and place it in the same directory as the XMRig executable.

Replace "YOUR_WALLET_ADDRESS" with your wallet address, and run the miner with sudo/administrator privileges.

Your MoneroOcean dashboard will be located at https://moneroocean.stream/

## Conclusion
Thanks for reading, and hopefully this helped you.
