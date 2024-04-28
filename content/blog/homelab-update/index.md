---
title: "Homelab Update"
date: 2024-04-27T09:00:28-05:00
tags: [tech, homelab]
summary: Have some old hardware lying around? Use it to start your new homelab.
toc: false
draft: false
---

Some time last year I wrote about using a cheap [Lenovo Thinkcentre](https://www.stacksocial.com/sales/lenovo-thinkcentre-m900-tiny-core-i5-6500t-16gb-256gb-ssd-wi-fi-windows-10-pro-refurbished) I bought as a lab machine to run my [homelab](https://www.reddit.com/r/homelab/wiki/introduction/) server. Initially I used it to [try out a new (to me) Linux distro](/linux-poll/), which I installed straight onto the machine. I enjoyed test driving it, but it never replaced my primary system.

So, this week I decided to repurpose the ThinkCentre as a general lab server to locally host open-source applications and dust off some of my brain's cobwebs around server configs and networking.

[This YouTube video from TechHut](https://youtu.be/olUD_F37n0E?si=zmN2r9tcmL9jTKta) provides a really easy way to get set up if you're interested in doing something similar.

For now I'm running [Ubuntu Server LTS](https://ubuntu.com/download/server) with [Docker](https://www.docker.com) and [Portainer](https://www.portainer.io/) for container management.

On top of this, I installed [Cosmos](https://cosmos-cloud.io/) as a dashboard which looks nice and has a really decent OOTB feature set. So far, I dig it.

{{< figure
img="cosmos.png"
caption="A tiny view of the Cosmos dashboard. The default color scheme reminds me of Mardi Gras."
command="Resize"
options="600x" >}}

Future plans include trying out some new apps (*this sure beats more software subscriptions*) and adding a [NAS](https://www.howtogeek.com/742893/what-is-a-nas/) to the lab, so if you have any recommendations send me an email reply using the button below.