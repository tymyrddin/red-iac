# Install a Kali VM

Kali Linux (formerly known as BackTrack Linux) is an open-source, Debian-based Linux distribution aimed at advanced Penetration Testing and Security Auditing. Kali Linux contains several hundred tools targeted towards various information security tasks, such as Penetration Testing, Security Research, Computer Forensics and Reverse Engineering.

## Why virtualisation?

* Pentesting needs a lot of practice before you actually approach a client to do the same on their live system.
* It provides a simulated environment, your main system is not touched. If you break your operating system by mistake while experimenting with any hacking-related tools, it happens inside your virtual system. You can reinstall the damaged operating system again.
* We have to [stay within the law—always](purple:index). We must practice our hacking-related tools in a legal way on our own systems.
* You can safely browse any websites in a virtual environment. If some malicious code enters into your simulated environment, let it stay; it won’t touch your main system. You can do every type of testing on it. 

## Which hypervisor?

* Although maintenance of VirtualBox leaves a lot to wish for, it is easy to install and can run on any system, and is therefor recommended as the best security lab solution for beginners.
* KVM is good for Linux. It is what I am using.
* For Windows, VMware is a good solution. Virtual PC is also good, but you cannot run Linux distributions inside it.
* For macOS, both VMware and Virtual PC are good options, including QEMU and Parallels.

## Installing hypervisor

Download the required hypervisor packages (including their dependencies) and then install them according to the nature of your OS.

As an example, installing VirtualBox on Ubuntu. You can install VirtualBox from the software center directly without opening up the terminal or issuing any command.

From the command-line:

    sudo apt install virtualbox virtualbox-ext-pack

It will not be the latest version. If you want to use the latest version of VirtualBox on Ubuntu, the easiest way would be to [download and use the deb file from Oracle’s website](https://www.virtualbox.org/wiki/Linux_Downloads). Double click on it to install it. 

## Installing Kali box

Use the [Official Kali VM's](https://www.kali.org/get-kali/#kali-virtual-machines). The docs are pretty clear.

## Dockers

You can also use dockers:

* [kalilinux/kali-rolling](https://hub.docker.com/r/kalilinux/kali-rolling)
* [kalilinux/kali-bleeding-edge](https://hub.docker.com/r/kalilinux/kali-bleeding-edge)

