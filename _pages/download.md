---
permalink: /download/
title: "Download"
layout: home
---
[![Tip Me via PayPal](https://img.shields.io/badge/PayPal-tip%20me-1462ab.svg?logo=paypal)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=YHB854YHPJCU8&item_name=Donation+pyTranscriber&currency_code=BRL)
[![Tip Me via Bitcoin](https://img.shields.io/badge/Bitcoin-tip%20me-f7931a.svg?logo=bitcoin)](https://github.com/raryelcostasouza/pyTranscriber/raw/master/doc/btc.png)
[![Tip Me via Ethereum](https://img.shields.io/badge/Ethereum-tip%20me-1462ab.svg?logo=ethereum)](https://github.com/raryelcostasouza/pyTranscriber/raw/master/doc/eth.png)
[![Tip Me via Litecoin](https://img.shields.io/badge/Litecoin-tip%20me-f7931a.svg?logo=litecoin)](https://github.com/raryelcostasouza/pyTranscriber/raw/master/doc/ltc.png)
[![Tip Me via BNB](https://img.shields.io/badge/BNB-tip%20me-1462ab.svg?logo=binance)](https://github.com/raryelcostasouza/pyTranscriber/raw/master/doc/bnb.png)
[![Tip Me via Dogecoin](https://img.shields.io/badge/Dogecoin-tip%20me-f7931a.svg?logo=dogecoin)](https://github.com/raryelcostasouza/pyTranscriber/raw/master/doc/doge.png)

pyTranscriber is developed as a hobby and is available for free, but donations are welcomed and essential for further improvements.

Your donations will help me free up my time to do more direct work on pyTranscriber. If I can generate more income from sponsorship here, I can take time out of other jobs and commit more time to work on <b>bug fixes</b>, add <b>new features</b>, and make <b>new releases</b>, like possible future integration with Mozilla Deep Speech engine, which may improve accuracy and control over the speech detection.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/A0A6AIR3D)
<iframe src="https://github.com/sponsors/raryelcostasouza/button" title="Sponsor raryelcostasouza" height="35" width="116" style="border: 0;"></iframe>

# For users living where Google Services are blocked:

For users in mainland China or other places where Google is blocked
The app will show a failure to connect to the internet message... meaning Google Servers.
You need to install a desktop VPN app like Windscribe to bypass the blockage and be able to use pyTranscriber.
对于中国大陆或其他谷歌被屏蔽的地方的用户
该应用程序将显示连接到互联网消息失败...意思是谷歌服务器。
您需要使用代理服务并在 pytranscriber 设置 > 代理中进行设置，或者安装桌面 VPN 应用程序（如 Windscribe）绕过阻塞并能够使用 pyTranscriber。

# 21/12/2022 - New stable version 1.9!
1. Windows/Linux version compiled with Nuitka (https://github.com/Nuitka/Nuitka) instead of pyInstaller to improve stability and fix random crashes while transcribing audio. If you still experience issues please report at Issues section.
2. Support for Ogg/ogv/mkv/webm media files on file selector


# 17/08/2022 - New stable version 1.8!!
1. Fixed bug: language codes for Chinese Languages updated accordingly to Speech API. Changed to "cmn-Hans-CN" and "cmn-Hant-TW" instead of "zh / zh-TW").. The output was always mistakenly coming in Cantonese (yue-Hant-HK). Now they come properly in Traditional Chinese and Simplified Chinese. Thanks to "Specter Hi" for reporting!
2. Added GUI language switch feature
3. Updated link to funding campaign at GitHub Sponsors

# 15/08/2022 - New stable version 1.7!!!
1. add proxy setting
2. add requirements.txt
3. rebuilt using pyInstaller 5.3 - more stability to prevent multithreading crashes on Windows
4. Added pipfile

<br>
# Windows
  * <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-win-installer.exe">pyTranscriber-windows-installer.exe</a>
  * <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-win-portable.zip">pyTranscriber-windows-portable.zip</a>

<a href="https://s.click.aliexpress.com/e/_Dm4YNnt?bz=300*250" target="_parent"><img width="725" height="90" src="https://ae01.alicdn.com/kf/S3619e57974f148d087c950fe497cdf55q/300x250.jpg" /></a>

<br>
# Windows 7 - If you had trouble using the latest version on Win 7 try this one...
  * <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.5-stable/pyTranscriber-v1.5-win7-installer.exe">pyTranscriber-v1.5-win7-installer.exe</a>
  * <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.5-stable/pyTranscriber-v1.5-win7-portable.zip">pyTranscriber-v1.5-win7-portable.zip</a>

<a href="https://s.click.aliexpress.com/e/_DEhY1iR?bz=725*90" target="_parent"><img width="725" height="90" src="//ae01.alicdn.com/kf/H1e303fdae72d4e4e9e7eafdcc327314ci.png" /></a>

<br>
# Mac
  * <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-mac.zip">pyTranscriber-mac.zip</a>

<br>
As the app is not downloaded from the AppStore, it may be necessary to allow it to run manually at
System Preferences > Security and Privacy

FOR macOS CATALINA AND ABOVE:
Open a Terminal and type the following command to add an exception allowing the app to run:

xattr -cr Downloads/pyTranscriber.app

  
# Linux 

For latest distros with GLIBC version 2.35 or higher download

* <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-linux-installer.zip">pyTranscriber-linux-installer.zip</a>
* <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-linux-portable.zip">pyTranscriber-linux-portable.zip</a>

For older distros or GLIBC version < 2.35 (incompatible with GNOME 40+)
  
* <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-linux-libc2.31-installer.zip">pyTranscriber-linux-lib2.31-installer.zip</a>
* <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-linux-libc2.31portable.zip">pyTranscriber-linux-libc2.31-portable.zip</a>


# License

This app and its usage are licensed under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GPL v3</a> license.
