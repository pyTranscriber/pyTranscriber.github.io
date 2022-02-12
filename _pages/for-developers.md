---
permalink: /for-developers/
title: "For Developers"
layout: home
---

This app consists basically of a friendly pyQt5 graphical interface for a customized version of <a href="https://github.com/agermanidis/autosub">Autosub 0.4.0</a> that can run on Linux, Windows and MacOS. All the hard work of processing the audio and generating the subtitles is done by Autosub.

# Dependencies
<br>1. pip3 install --user pyQt5
<br>2. pip3 install --user autosub
<br>3. pip3 install --user pyinstaller (only for generating bundled binary)
<br>4. Download the static ffmpeg binary and put on project root folder or install system wide

<br>
# How to run?
$ python3 main.py

<br>
# How to edit the GUI?
Install Qt5 Designer and open the file pytranscriber/gui/gui.ui

<br>
# How to convert the .ui file (qt5designer project file) to .py?
$ pyuic5 gui.ui -o gui.py

<br>
# How to generate the python bundled binary package version?
$ pyinstaller --add-data "lib/google_api_python_client-1.12.8.dist-info/*;google_api_python_client-1.12.8.dist-info" --clean main.py

The output binary will be on subfolder dist/main and has all dependencies included. For more details check pyinstaller documentation

Note: At least in my Manjaro system running latest python I need to add some extra parameters like as follows to be able to run the generated binary:
<br><br>
$ pyinstaller --onefile main.py --hidden-import='packaging.version' --hidden-import='packaging.specifiers' --hidden-import='packaging.requirements'

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
