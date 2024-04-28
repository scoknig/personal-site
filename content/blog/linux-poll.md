---
title: "Using Data to Choose a Linux Distro"
date: 2023-07-07T16:51:29-05:00
tags: [data, tech, homelab]
summary: An interesting data exercise I ran with with the Mastodon community.
toc: false
draft: false
---

## The Problem

I recently decided that I wanted to beef up my home lab a bit by adding a small, inexpensive machine that I can use as a sandbox for server projects and testing operating systems. When I realized that StackSocial had a [Lenovo ThinkCentre M900](https://stacksocial.com/sales/lenovo-thinkcentre-m900-tiny-core-i5-6500t-16gb-256gb-ssd-wi-fi-windows-10-pro-refurbished) on sale for less than $200, I ordered one.

I also knew I wanted to try something besides Windows and MacOS on this new machine, so I decided to evaluate Linux distros. As it turns out, choosing a Linux distro is a really tall order for someone who's only superifically familiar with the domain; there are hundreds, if not thousands, of distributions.

So, knowing the membership to be Linux and FOSS fans, I turned to the Mastodon community to help me decide what to try out first.

## Data Collection

I [posted a poll](https://fosstodon.org/@scoknig/110634616581420265) on Mastodon asking everyone to vote for their favorite Linux Distro. 

I didn't expect to get much engagement as a new member with few followers, but it seems as though this topic is something everyone has an opinion on.

Having set the poll to stay open for a week, I received 58 votes, not accounting for recommendations from replies on the post (I asked everyone with an "Other" vote to specify their preference in a reply).

After a week, I combed through the comments to create the full dataset analyze the results.

## Analysis

I used a Jupyter Notebook for the basic analysis. Pandas helped me to import and transform the data, and I used Matplotlib for the visualizations. As there were two types of recommendations, I classified the recommendations as either __distros__ or __desktops__ ([what's the difference?](https://embeddedinventor.com/linux-distros-vs-desktop-environments-differences-explained/)).

From there, I added a few blocks of code to clean things up, sort the data, and create the bar charts.

## Results

Now that I had a couple of visuals to evaluate, the results were quite interesting and unexpected. [Zorin OS](https://zorin.com/os/) was one of my personal preferences going into the poll, but it hadn't received a single vote (since the poll closed, I've had some comments recommending it).

[Linux Mint](https://linuxmint.com/) was by far the winner in the distro category, followed by [Fedora](https://www.fedoraproject.org/) and [NixOS](https://nixos.org/). So, it looks like I'll be starting off with Linux Mint.

For desktop environments, [KDE Plasma](https://kde.org/plasma-desktop/) was the most recommended.

I've since [posted the results on Mastodon](https://fosstodon.org/@scoknig/110674998281361161), in case anyone who participated was interested in the overall outcome.

I've pushed the project files to my [Github](https://github.com/scoknig/mastodon-linux-recs/blob/main/Linux%20Poll%20Analysis.ipynb), but I recommend [checking it out here](https://nbviewer.org/github/scoknig/mastodon-linux-recs/blob/main/Linux%20Poll%20Analysis.ipynb) using the Jupyter Notebook Viewer if you just want to see the results.