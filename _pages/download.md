---
permalink: /download/
title: "Download"
layout: home
---
[![Tip Me via PayPal](https://img.shields.io/badge/PayPal-tip%20me-1462ab.svg?logo=paypal)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=YHB854YHPJCU8&item_name=Donation+pyTranscriber&currency_code=BRL)
[![Tip Me via Bitcoin](https://img.shields.io/badge/Bitcoin%20Lightning-tip%20me-f7931a.svg?logo=lightning)](https://github.com/raryelcostasouza/pyTranscriber/raw/master/doc/lightning.jpeg)

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

# Hashes to verify the files authenticity (SHA256 sum):

## Windows:

pyTranscriber-1.9-win-installer.exe - 245e6947859e25d97ba49a27fc3f58d195ce7f266b71f8dc020800b17645c45e
pyTranscriber-v1.9-win-portable.zip - 503677359734ad7c0cd673295149d090cfb8977821874983819ff2ca57e97d56

## MacOS

pyTranscriber-v1.9-mac.zip - ca0a4c5a41561b94034156f0bdff6e4388d66d01bf0f8455e4451f80c87e55e4

## Linux

pyTranscriber-v1.9-linux-portable.zip - f76cdda1ca24868b5a7d5aeeee4a1763d455e033c4a16822b5782505d738b797
pyTranscriber-v1.9-linux-installer.zip - 29f0ec7ad46b0f6328258cad8ce4ce977842f73ca2e98e3bc92b9cc37b661ded
pyTranscriber-v1.9-linux-libc2.31-installer.zip - 6411c38eac98fb3a4b035cd99d7f73fa61375f66426ce0c5ffd7ceee7bf184b6
pyTranscriber-v1.9-linux-libc2.31-portable.zip - 3bf3155c026eaa24138fada830d673cb4332216e51fcb24c7c6a3d6aac23e341

<br>
# Windows
  * <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-1.9-win-installer.exe">pyTranscriber-windows-installer.exe</a>
  * <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-win-portable.zip">pyTranscriber-windows-portable.zip</a>

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
* <a href="https://github.com/raryelcostasouza/pyTranscriber/releases/download/v1.9/pyTranscriber-v1.9-linux-libc2.31-portable.zip">pyTranscriber-linux-libc2.31-portable.zip</a>



# License

This app and its usage are licensed under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GPL v3</a> license.
