## GameServerKernel / Scripts
This repo will be used for support/provide GameServerKernel for Linux - **1000HZ & 100HZ**

### [.config file here - 1000HZ](https://raw.githubusercontent.com/MikkelDK/GameServerKernel/master/config)

**Remember to rename "config" to ".config" on your server, if you want to re-compile with other HZ (E.g: 100HZ!)**

### Rates / Script to gameserver:
(**This rates is for CSGO Server!**) - Test it out, it's recommend to test:
[Rates is here](https://raw.githubusercontent.com/MikkelDK/GameServerKernel/master/rates.cfg)

Script to your linuxserver:
[/root/script.sh](https://raw.githubusercontent.com/MikkelDK/GameServerKernel/master/script.sh)
```
apt-get install tuned && apt-get install tuned-adm
```
tuned-adm profile latency-performance **//NOTE: You don't need tuned-adm, if you are using Ryzen 7 3700X/3800X/3900X**

### Unix Support:
Debian / Ubuntu 64bit.

CentOS/Other Unix should be supported! **Not tested!**

## (Release): [Download](https://github.com/MikkelDK/GameServerKernel/releases/download/3.0-1000hz/Kernelv3.zip) - (1000HZ - Kernel: 5.2.14 with LowLatency & NFP)

## (Release): [Download](https://github.com/MikkelDK/GameServerKernel/releases/download/v3.1-1000hz/kernelv3.1.zip) - (1000HZ - Kernel: 5.3.8 - LowLatency Only!)

## (Release): [Download](https://github.com/MikkelDK/GameServerKernel/releases/download/v3.0-100hz/Kernelv3.0-LLY-100hz.zip) - (100HZ LowLatency Only - Kernel: 5.3.8)

### What does NFP/LLY means?
LLY => **Low-Latency** (Stable Tickrate & High Performance for your **GAMESERVER**) **ONLY 100HZ & 1000HZ having LLY!**

NFP => **No-Fored-Preemption** (Run as many gs you can as possible on your hardware!) **ONLY 1000HZ having NFP!**

### Screenshots of Net_Graphs:
If you are using **LLY config** - It will be looks between: **0.000-0.900 VAR** (Depends how many slots is setup to be used!)
1st screenshot is from i9-9900K (No matter, about you are using Ryzen 7 3700X/i9-9900K)
![This is happens if server is running with Ryzen 7 3700X/i9-9900K](https://i.gyazo.com/c1d31dcfad0f616b7c66df09693a94c7.jpg)

2nd screenshot is from i9-9900K (No matter, about you are using Tuned-adm profile latency-performance!)
![second](https://i.gyazo.com/e615db5f3b73c14e6ed16d42cee96e1b.jpg)

**Overall, depends CPU so it's _POSSIBLE_ to run 0.000-0.001 if it's match/retake/scrim servers!**

**If you are planned to host 25slots FFA/DM Server. it can jump between: 0.000-0.900**
