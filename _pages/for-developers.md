---
permalink: /for-developers/
title: "For Developers"
layout: home
---

# See the code

<a href="https://github.com/raryelcostasouza/pyTranscriber">pyTranscriber App Github Repository</a>

This app consists basically of a friendly pyQt5 graphical interface for a customized version of <a href="https://github.com/agermanidis/autosub">Autosub 0.4.0</a> that can run on Linux, Windows and MacOS. All the hard work of processing the audio and generating the subtitles is done by Autosub.

# Dependencies
<br>0. <b>Python 3.8 </b>
<br>1. pip3 install pipenv
<br>2. pipenv install (install all dependencies from Pipfile)
<br>3. Download the static ffmpeg binary and put on project root folder

<br>
# How to run?
$ pipenv shell
$ python3 main.py

<br>
# How to edit the GUI?
Install Qt5 Designer and open the file pytranscriber/gui/gui.ui

<br>
# How to convert the .ui file (qt5designer project file) to .py?
$ pyuic5 gui.ui -o gui.py

<br>
# How to generate the python bundled binary package version with ffmpeg included?

# Linux:
$ pyinstaller main.py --path="$(pwd)" --add-binary="ffmpeg:." --onefile --clean

# Windows:
$ pyinstaller main.py --path=$pwd --add-binary="ffmpeg.exe;." --onefile --clean

# Mac:
$ pyinstaller main.py --path="$(pwd)" --add-binary="ffmpeg:." --clean --windowed

The output binary will be on subfolder dist/main and has all dependencies included. For more details check pyinstaller documentation
<br>
# On Linux how to generate a statically linked binary so it can run even on systems with older glibc installed?

As explained in <a href="https://github.com/pyinstaller/pyinstaller/wiki/FAQ">pyInstaller-FAQ</a>:

> The executable that PyInstaller builds is not fully static, in that it still depends on the system libc. Under Linux, the ABI of GLIBC is backward compatible, but not forward compatible. So if you link against a newer GLIBC, you can't run the resulting executable on an older system.
<br><br>
> <b>Solution 1)</b>To compile the Python interpreter with its modules (and also probably bootloader) on the oldest system you have around, so that it gets linked with the oldest version of GLIBC.
<br><br>
> <b>Solution 2)</b> to use a tool like StaticX to create a fully-static bundled version of your PyInstaller application. StaticX bundles all dependencies, including libc and ld.so. (Python code :arrow_right: PyInstaller :arrow_right: StaticX :arrow_right: Fully-static application)"
<br>

<br>
# Install staticx and patchelf (dependency)</b>

$ pip3 install --user patchelf-wrapper

$ pip3 install --user staticx

<br>
# After generating the binary with pyinstaller, open the dist folder and run:

$ staticx main main-static

The newly created main-static contains all library dependencies, including glibc, so it should be able to run even on very old systems.

Note: In my Manjaro system the first time I run this command I got an error related to "libmpdec.so.2 => not found". Installing the package <b>mpdecimal</b> on the package manager solved the issue.
