---
title: 'FAQ'
taxonomy:
    category:
        - docs
visible: true
---

## ParrotOS Frequently Asked Questions

### Why should I use ParrotOS?

Penetration testing is a time intensive job, maintaining your toolkit shouldn't 
be also. We make it easier for professionals to accomplish the important stuff 
by reducing the time and effort wasted making sure their tools work.

Not sure if Parrot is for you? Check out "[Should I use Parrot?](https://docs.parrotlinux.org/intro/what-is-parrot/#should-i-use-parrot)" to be sure.

### What is the default live password?

Live user: **user**
Live pass: **toor**

Parrot may not have a root password since Parrot 4.4, to launch programs as root or to obtain a root terminal, use **sudo**

### How do I upgrade my system?

First please, do __NOT__ use `apt-get upgrade`. Because ParrotOS is a rolling distribution and how APT works, the command will cause considerable problems to your system. We don't recommend `apt-get` in general as the command is not really meant for end-users. The following are the recommended ways to update your system:

1) First method

Open a terminal window (default is Alt+T) and launch the following command:

```text
sudo parrot-upgrade
```

2) Second method

Open a terminal window and launch the following commands:

```text
sudo apt update
sudo apt full-upgrade
```

3) Third method

Open System > Administration > Package Manager (synaptic)

Then click on the button to update the packages list.

Click on the other button to select the upgrades and finally apply the changes.

### Why isn't $toolname installed?

We have a set of prerequisites to check before a tool makes its way into our repositories such as:

- Is the tool actively maintained?

- Does it have the necessary documentation?

- Is it FLOSS, FOSS or does it's license allow redistribution?

- Are there other tools that do the same thing?

- Is there someone available to package and maintain it?


and more[...];


If the answers were “Yes” we're more than glad to take your request via our [Community Portal](https://community.parrot.sh/c/development).


### Where can bugs be submitted?

If the bug involves a specific piece of software maintained by Parrot, then search the project on our [Dev Portal](https://nest.parrot.sh/) and open an issue.

If the bug involves a software package that is not listed, then you should contact the maintainer of that particular software.

If you are not sure what software is involved, or if you don't know how to contact the upstream developer, then contact us on our [Community Portal](https://community.parrot.sh/c/development/)

### What should my sources.list look like?

`/etc/apt/sources.list` should be **EMPTY**

`/etc/apt/sources.list.d/parrot.list` should contain the following content

```bash
deb https://deb.parrot.sh/parrot/ rolling main contrib non-free
#deb-src https://deb.parrot.sh/parrot/ rolling main contrib non-free
deb https://deb.parrot.sh/parrot/ rolling-security main contrib non-free
#deb-src https://deb.parrot.sh/parrot/ rolling-security main contrib non-free
```


### The installer wants a CD/DVD but I'm using a USB drive.

If this happens, then you did something terribly wrong during the creation of the USB bootable device.

This usually happens when you use software that doesn't respect the isohybrid standards.

The following page will describe the issue, how to fix it and why it can occur.

[Create a Boot Device](https://docs.parrotlinux.org/getting-started/create-boot-device/)

### How do I prepare a bootable Parrot USB drive?

1) Download Etcher from our [Download page](https://parrotlinux.org/download.php) or directly from [www.etcher.io](https://www.etcher.io).

2) Download the ISO file of the Parrot version you need from our our [Download Page](https://parrotlinux.org/download.php)

3) Use Etcher to flash the ISO file into a free pen drive (the pen drive will be erased).

Read more [here](https://docs.parrotlinux.org/getting-started/create-boot-device).

### I'm new to Linux, please help me!

Of Course! Please check out [helpme](https://docs.parrotlinux.org/library/helpme/), the [Using ParrotOS](https://docs.parrotlinux.org/info/start/) pages and the [further reading](https://docs.parrotlinux.org/library/start/). We also strongly recommend taking the [EdX course](https://www.edx.org/course/introduction-to-linux/) by the [Linux Foundation](https://www.linuxfoundation.org/).

### Should I encrypt my harddrive?

Yes, always. Do it during your initial install or you will need to reinstall. 

### My hardware is *xyz-super-cool gizmo . . .* will it run ParrotOS?

Maybe, check our [supported hardware](https://docs.parrotlinux.org/trbl/supported-hardware/) page.

### Can you teach me how to hack, become a Linux uber-duber user, or live a holy life like Cucumber Bob?

Uh no. Nooope. . . You do not know deh way. <br>Seriously, [reading](https://docs.parrotlinux.org/library/start/) will lead you down the path of autodidactic salvation.

### How can I disable the GUI update reminder? 

Please see [here](https://community.parrot.sh/t/parrot-updater/1485/2)

### I can't login at startup as root?

That is by design, use `sudo` instead.

### How do I setup auto-login?

Our OVA images are already configured for auto-login (any passwords needed are on the desktop). We don't recommend or support auto-login for our other builds.

### Does Parrot Replace Heads/Tails?

No, although similar Parrot isn't designed to replace or be used as a Heads/Tails system.

### What is the difference between Kali Linux and ParrotOS? 

There are several and we think you should try both to really get a solid feeling of which one fits you best. 

### Can I contribute to this FAQ?

Of course! The pages are written in Markdown and can be accessed [here](https://nest.parrotsec.org/parrot-organization/documentation/blob/master/docs/faq.md).


&nbsp;

&nbsp;

[Using Parrot](https://docs.parrotlinux.org/info/start/) | [Troubleshooting](https://docs.parrotlinux.org/trbl/start/) | [Linux Beginner Guide](https://docs.parrotlinux.org/library/lbg-basics/) | [Home](https://docs.parrotlinux.org/)