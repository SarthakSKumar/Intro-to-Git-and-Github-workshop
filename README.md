## Upcoming Workshop

<!-- [Register Here](https://intro-to-git-may-2018.eventbrite.com.au/) -->



**Location**

ERC, Building 171, Level 3, Rooms 329 & 330

[Visual Guide to Workshop Location from Swanston Tram Stop](https://tinyurl.com/tram2colab)

[Visual Guide to Workshop Location from House of Cards](https://tinyurl.com/coffee2colab)



## Table of Contents

* [Introduction](#introduction)
* [Workshop Requirements](#workshop-requirements)
* [Text Editors](#text-editors)
* [Installing Git](#installing-git)
* [Seeking Help](#seeking-help)


Introduction
----

Thank you for your interest in Git!
The information in this page is for people attending an
_Introduction to Git and GitHub_ workshop with Research Platforms at University of Melbourne.

Git is a system for managing snapshots of plain text projects.
It is widely used in industry and academia for distributed collaboration amongst programmers.
It is also useful to individuals who want to manage and back up plain text projects across multiple devices.
GitHub is a popular website for hosting projects that use Git.

This workshop will provide a gentle introduction to Git and GitHub aimed at a general audience.
Since Git is most often used in a text-based environment,
we will also cover some simple use of the Unix command line.
The goal of the workshop is that you will attain some idea of what Git is and how to begin using it.


Workshop Requirements
----

It is easy for a workshop to get derailed by finicky technical issues caused by operating system differences or internet connection problems.
You have some responsibility for ensuring you meet the workshop requirements.

Please do the right thing by other attendees:

**You must have all software installed and an internet connection established before the workshop begins.**


### Internet Connection

Anyone from University of Melbourne will probably connect using UniWireless.

If you are from another university, _please arrive early_ to establish your EduRoam connection.

In case you cannot connect to UniWireless or EduRoam,
you should bring a device that can act as a hotspot.
Most internet-enabled smartphones work well for this purpose.
So long as you install all the required software ahead of time,
the workshop will not require much download or upload expenditure.


### Required Software

You will need software for editing plain text files and for using Git.
More detailed software suggestions and instructions are below.

You must have the software downloaded before the workshop.

You should also do some basic sanity checks to ensure that it works correctly.
At a minimum, you must be able to open a terminal and run `git --version` without seeing any errors.
You must also be able to edit plain text files.


Text Editors
----

The workshop will require you to have access to a _plain text editor_.
Some common text editors include Notepad, Eclipse, Atom, Vim and Emacs.
Some text editors are easier to use than others,
and some offer more features.

Notepad is easy to use but has minimal features.
Vim and Emacs are hard for beginners to use, but they become more and more powerful with experience.

For this workshop, we recommend [Atom](https://atom.io).

Atom is a free, open source and cross platform text editor.
It looks very pretty, it is very customisable with a lot of features and plugins available,
it is easy to install, and it will work on everyone's laptop.
You will be able to keep using it after the workshop is over, forever, without paying anything.

If you already have some other preferred text editor,
you may choose to use that in the workshop.
However, if you run into problems, it is possible that no one will know how to help you.
Furthermore, you might take workshop time away from the intended material,
which is not fair on other attendees.

So, only use an alternative text editor if you feel confident that you can solve any problems that could arise.

**Note:** Do _not_ use a product such as Microsoft Word.
A word processor is not the same as a text editor.
The distinction will be explored in more detail in the workshop itself.


Installing Git
----

Although Git is cross platform,
each operating system offers different installation methods.
We are still evaluating which methods will be optimal for our workshops.

Have a look through the available options and choose one that seems suitable to you.
You may need to try more than one to find a good fit for you and your system.

* [Windows](#windows)
* [Mac OS X](#mac)
* [Linux](#linux)


### Windows

There are two or three main ways to install Git in Windows,
depending on which version of Windows you are running.


#### Git for Windows

This is the easiest but least powerful method.
Download the installer from https://git-for-windows.github.io/ and run it.

You will be offered several options.
The default options should be safe.
The following screenshots show the options we tested with.

![](./figures/Installation_options.jpg)

![](./figures/lineendingconversion.jpg)

![](./figures/OpenSSL.jpg)

![](./figures/terminalemulator.jpg)

![](./figures/configuringextraoptions.jpg)


#### Cygwin

Cygwin is a Unix environment for Windows.
It is very powerful, but it can be a little tiresome to install.
Its website is [http://cygwin.com/](http://cygwin.com/).

When installing Cygwin, you are offered a choice of a large number of packages to install with it.
You probably don't want to install all of them, since it will take too long to download them all,
and most of them will just sit there taking up hard drive space without ever getting used.

For the workshop, you will want the following packages:

* Everything in `base`.
* The packages `devel/git`, `net/openssl`, `doc/man-db` and `doc/man-pages-posix`.
* The package `xxd`.


#### Ubuntu for Windows 10

This is the most powerful method, but it is quite complicated to set up.
It offers a Linux-like environment within Windows 10.

Before you proceed with this method,
you should know that Linux is an operating system often used in small devices like wifi routers and Android phones,
and large high-performance servers.

[Ubuntu](https://www.ubuntu.com/) is a Linux _distribution_,
meaning a collection of software that can manage what is installed on a Linux system.
There are a lot of Linux distributions;
Ubuntu is often recommended to people who are new to Linux.

Normally Linux and Windows programs don't work well together.
When _Ubuntu for Windows 10_ is activated,
it acts as a translator between Linux and Windows,
so now they can work with each other.

If you want to use this method for installing Git,
you should first [activate Ubuntu for Windows by following this tutorial](http://www.omgubuntu.co.uk/2016/08/enable-bash-windows-10-anniversary-update).

Once you have your Ubuntu environment active,
you will need to install Git by running:

~~~
sudo apt-get install git
~~~

We have not tested it, but you possibly also need to install Atom from within Ubuntu:

~~~
sudo apt-get install atom
~~~


### Mac OS X

For the workshop, we will be using Git on the command line in a terminal.
Fortunately, all Macs come with a terminal program.

Unfortunately, it is not obvious how to find it.
Many Mac users don't even know they already have this extremely powerful tool at their fingertips, ready to go.

[This tutorial by Jim Hoskins](http://blog.teamtreehouse.com/introduction-to-the-mac-os-x-command-line)
provides an introduction to the terminal in Mac OS X,
including how to find and open it.

Once you can open a terminal,
there are multiple methods for installing Git.
[These instructions summarise the available methods.](https://www.atlassian.com/git/tutorials/install-git#mac-os-x)

The XCode method is probably simplest, although it is a very large download.
Homebrew is a popular alternative.


### Linux

Since Git is used to version control Linux itself,
most Linux distributions make it very easy to install Git.

If you are attending the workshop with a Debian-like laptop (for example, if it
is running Ubuntu or Mint), you can install Git using _Synaptic_,
which is a graphical interface for package management.
You can hopefully find Synaptic in the menus offered by your desktop environment.

To install Git from the command line in either Debian-like or Red Hat-like
systems, see instructions [here](https://www.atlassian.com/git/tutorials/install-git#linux).

If you are running some other distribution,
you probably know what you are doing and can find your own help :)


Seeking Help
----

The workshop instructor has a lot of experience with Linux,
a little out-dated experience with Windows,
and no experience whatsoever with Mac OS X.
Therefore, the instructor's ability to solve problems you encounter on Macs and Windows
would probably just amount to doing a bunch of Googling for you.

Furthermore, the workshop instructor needs to dedicate their time and energy to
developing workshop material, not acting as a helpdesk ;)

So, if you face some challenges when installing Git,
please do your own Googling _first_,
before contacting the workshop instructor for tech support.

However, if you have a problem that you just can't solve even after serious Googling for an hour or two,
please definitely contact the instructor as soon as possible!
We hope you can feel empowered to solve problems independently,
but we don't want you to frustratedly bang your head against the wall for days :)

* [Email](mailto:terice@unimelb.edu.au)
* [Twitter](https://twitter.com/resnomicon)

See you at the workshop!


References
----

https://github.com/cryptarch/sgit.git
https://daringfireball.net/projects/markdown/

Github Cheat Sheet for Markdown: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

CC Licence: https://raw.githubusercontent.com/resbaz/intro-git-workshop/master/LICENSE.md

http://phdcomics.com/comics/archive/phd101212s.gif

http://swcarpentry.github.io/git-novice/02-setup/
