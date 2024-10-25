# InnoSetup Updater

[![Latest Version](https://img.shields.io/github/release/Wilenty/InnoSetup-Updater.svg)](https://github.com/Wilenty/InnoSetup-Updater/releases/latest)
[![Total Downloads](https://img.shields.io/github/downloads/Wilenty/InnoSetup-Updater/total.svg)](https://github.com/Wilenty/InnoSetup-Updater/releases)
[![Latest Release Downloads](https://img.shields.io/github/downloads/Wilenty/InnoSetup-Updater/latest/total.svg)](https://github.com/Wilenty/InnoSetup-Updater/releases/latest)

I made this program, because I could not find a program of this type, for that I found information that the main developer does not plan to add such functionality at all:
https://groups.google.com/g/innosetup/c/y7Xgp-gyMkQ/m/17vCpPSAAQAJ
but he suggests  to use "winget" that even some users of InnoSetup forum don't know it:
https://groups.google.com/g/innosetup/c/y7Xgp-gyMkQ/m/QgGV7JqdAwAJ
Since there are questions on the Internet about such functionality, I decided to try to create one.

It does not download and install any version of InnoSetup if you do not have it. You have to download it yourself the first time and install or unpack the portable version. I'm assuming you want to check if a new version has been released to adjust your installer to it.

It works from Windows 7, because latest InnoSetup works from Windows 7, and it can update any version of InnoSetup (installed/portable) with a comfortable (InnoSetup) GUI.

It uses the Linux command-line "wget" program (compiled for Windows OS) to connect the InnoSetup website, because in the latest InnoSetup you have only three simple functions:
https://jrsoftware.org/ishelp/topic_isxfunc_downloadtemporaryfile.htm
https://jrsoftware.org/ishelp/topic_isxfunc_downloadtemporaryfiledate.htm
https://jrsoftware.org/ishelp/topic_isxfunc_downloadtemporaryfilesize.htm
and the size of latest InnoSetup, as they called "Tiny footprint: only 1.5 mB":
https://github.com/jrsoftware/issrc/blob/is-6_3_3/ISHelp/isetup.xml#L144
or in the future 6.4.0(-dev) version "Tiny footprint: only 1.75 mB":
https://github.com/jrsoftware/issrc/blob/d6d8def600395d1460a48aec3815189a4ac1b9ae/ISHelp/isetup.xml#L158
So, new InnoSetup it's bigger than my program + wget command-line program: 1,44 MB, and wget has a way lot more functionality than above three simple functions.

By the way,
I can hide the wget window at program start, but I intentionally showed it to you that you know "what's going on".
