---
title: "Personal Automations"
date: 2023-10-25T07:36:43-05:00
tags: [life, tech, homelab]
summary: How I automate some of the boring/tedious stuff in life.
toc: false
draft: false
---

Since I learned to code, I've always been a fan of eliminating boring and/or tedious stuff with automation. This can involve anything from custom scripting (usually with Python, in my case) to using a service like [IFTTT](https://ifttt.com/), [Zapier](https://zapier.com/), or [Make](https://www.make.com/en/integromat-evolves-to-make/) (formerly Integromat). With these tools you can connect most common services that expose an [API](https://www.ibm.com/topics/api/).

While automation use cases are usually born out of some personal pain point or specific challenge, I'm always interested in seeing what other people automate and how they choose do it. I've also taken great inspiration from pieces like Al Sweigart's [*Automate the Boring Stuff with Python*](https://automatetheboringstuff.com/) and [this classic Github repo](https://github.com/NARKOZ/hacker-scripts).

I recently bought an IFTTT subscription and audited my personal life for a list of things that take up too much time or involve a tedious process. 

Here are some of my favorites:

- **Email/SMS to Brag File (IFTTT)**: Sending an email or text to IFTTT creates a new row in my career [brag file](https://www.thefountaininstitute.com/blog/brag-documents) with text I include. (My "brag file" is what I humbly call the personal doc where I track my professional accomplishments so I don't forget about past wins.)

- **Blog RSS to Socials (IFTTT)**: Each time I publish a new post on this site, it gets automatically posted to my Twitter and Mastodon accounts. (Bonus---[Buttondown](https://buttondown.email/) also sends an RSS-driven email to readers subscribed to my posts)

- **Instapaper to Trello (IFTTT)**: New articles saved to Instapaper automatically get added to a "future blog posts" list on my personal Trello board.

- **Trello Board Automations (Trello)**: Using Trello's built-in automation capability, I've set up rules and buttons that keep my task board organized so I never lose track of any reminders, tasks, or projects. These are driven by due-dates, sources (cards added via email, etc.), and task age (highlighting overdue items and so on).

- **Smart Home/IoT Automations (IFTTT)**: Various applets turn on/off lights and appliances using smart plugs driven by my location, times, alarms, etc.

- **Custom Transaction Categorization (Python)**: A custom script I wrote using Python which can take a CSV export of my bank transactions and categorize them for my accounting. It can categorize a year's worth of transactions in less than a second, which is pretty neat. It's also more secure and private than granting access or uploading my bank info to some third-party company's database.

Is there anything useful or cool that you've automated? Send me an email, I'm interested to learn more about it!