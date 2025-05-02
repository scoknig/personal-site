---
title: "How to Keep Your Mac Awake Using Terminal"
date: 2025-05-01T18:54:22-05:00
tags: [tech]
summary: Using the 'caffeinate' command on MacOS.
toc: false
draft: false
---

Recently I was running some tasks on my Macbook Pro I wanted to prevent the machine from sleeping. A quick [DuckDuckGo](https://spreadprivacy.com/why-use-duckduckgo-instead-of-google/) search tipped me off to the `caffeinate` command that's built into the Terminal in macOS. If this is a well-known thing in macOS, I've never come across it so I thought I'd share here in case anyone else would find it useful.

If you have some reason to prevent your machine running macOS from sleeping, `caffeinate` gives you a few options. For basic usage, here's how you use it:

## Step 1: Open Terminal
If you're not sure how to do this, [see here](https://www.tomsguide.com/how-to/how-to-open-terminal-on-mac) (it's one of the Applications that comes with macOS).

## Step 2: Type `caffeinate` and hit Enter

This will prevent your Mac from sleeping as long as you don't close the lid or exit Terminal. Once you close Terminal, hit Ctrl+C, or close the lid on your machine, the process will exit and normal sleep behavior will resume.

Now, here's the really handy part—`caffeinate` takes arguments, meaning that if you add an option after the command, you can change how long it will run or set it to wait for a specific process or command to complete before exiting.

- `caffeinate -i` prevents sleeping indefinitely (prevents idle sleeping)
- `caffeinate -u -t 3600` prevents sleeping for 1 hour (the `-u` flag resets the last time the user was active, and `-t 3600` defines the time limit in seconds, equivalent to an hour)
- `caffeinate -s <command>` prevents sleeping until a command finishes running. Just replace `<command>` with your desired command
- `caffeinate -w <pid>` prevents sleeping until a running process completes, provided you define the PID of the process

---

### Resources
For further reading, here's [the original article](https://commandmasters.com/commands/caffeinate-osx/) I found as well as the actual [man page](https://ss64.com/mac/caffeinate.html) for the command.