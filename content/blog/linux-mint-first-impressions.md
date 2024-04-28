---
title: "A Week with Linux Mint"
date: 2023-07-14T15:31:48-05:00
tags: [tech, homelab]
summary: A few of my first impressions.
toc: false
draft: false
---

Last week I posted here about open-sourcing my decision on which Linux distribution to use on my new lab machine. The overwhelming majority voted for Linux Mint, so that's what I went with.

Not having used Linux in many years, I couldn't recall anything particularly good or bad about my experience with the OS. That is to say, I'm going into this with an open mind.

The hardware I'm using isn't anything special, which personally I prefer in the sense that it will allow me to additionally evaluate my chosen OS on an average system.

If you're interested, here are the basic specs:

- Model: Lenovo ThinkCentre M900 (2017, Refurbished)

- Processor: Core i5-6500T

- Processor speed: 2.5GHz

- Intel HD Graphics 4000

- RAM: 16GB

- Storage: 256GB

- vPro

- Support for USB 3.0

The intention here is that it will serve as part of my home lab on which I can run experiments and projects without affecting my primary machines. So, with that in mind, it should be sufficient for its purpose.

## Installation

I didn't have any major issues installing Linux Mint on the machine. LM provides detailed [installation docs](https://linuxmint-installation-guide.readthedocs.io/en/latest/) that were easy to follow, and the process was a standard one: create a bootable USB, boot it up using the BIOS, then install.

One thing I appreciated was that, when booting with the install media before the main installation, you're actually loading a live boot of Linux Mint, which allows you to preview and check for compatibility issues before you fully commit.

Once I ran the full installation, it probably took less than ten minutes to get fully set up. Another plus in my book.

By the way, I'm running __Linux Mint 21.1 "Vera"__.

## User Experience

The one challenge I had in getting things fully operational was setting up the wi-fi adapter drivers on the system. Unfortunately, the [Realtek RTL8188FTV](https://www.realtek.com/en/products/communications-network-ics/item/rtl8188ftv) that came with the ThinkCentre (the hardware does not have internal wi-fi support) was not recognized by the OS.

So, after some diligent research I was able to identify a solution that got it working. For those interested, I may write up a separate post on how specifically I accomplished this, but suffice it to say that it took some advanced tinkering to get things running. This is something that could be a major turn-off to 

This Github repo was critical in getting the drivers installed and adding the appropriate kernel modules: https://github.com/kelebek333/rtl8188fu

After that minor inconvenience, everything in general has been pretty smooth. The OS itself is snappy and efficient. The themes and color options are a nice touch for those who like customization.

The overall feel is similar to Windows, so it is not alien to someone who might be wanting to migrate to Linux from that domain. Many of the folder actions, start menus, and general functionality are akin to what you'd find in Windows. I've heard that Linux Mint is a good starter Linux experience for those coming from a strictly Windows background, and so far I say that notion holds up.

My only small gripe is that some of the software packages seem to be intentionally held back by the distro maintainers from the publisher's latest releases. For example, I wanted to set up the new *Supernova* release of [Thunderbird](https://www.thunderbird.net/en-US/), but at this time that does not appear to be possible. However, after some research I realized that this seems to be common practice in the Linux community and should not be unexpected. Some may see this as a negative, but I realize that this may also be a mechanism to protect against zero-day vulnerabilities as well as other issues by waiting a bit before integrating brand new releases. So for now, I'm okay waiting for a bit longer.

All things considered, the experience has been positive after one week. We'll see how things progress as I continue to build out the machine.