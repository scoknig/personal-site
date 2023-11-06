---
title: "How to Create Custom Terminal Commands in MacOS"
date: 2023-11-06T16:30:27-06:00
tags: [tech]
summary: Making automation easier with custom commands on MacOS.
toc: false
draft: false
---

I recently wrote here about some of my favorite [personal automations](/personal-automations/). When updating my a finance automation script recently, I decided I wanted a way to quickly run the automation anywhere. I typically have a terminal open, so I thought a custom terminal command would be the best way to fire off my scripts when I need them.

Unfortunately, the resources are slim out there regarding how to configure custom terminal commands in MacOS. Using an article I dug up (linked below), I was able to figure it out. 

Here's how I was able to get it set it up in a few steps:

## 1. Create a file to store your custom commands

Open a terminal window and navigate to the Home directory using the command:

```sh
cd ~
```

Now, create the custom commands file using the command:

```sh
touch .my_custom_commands.sh
```

## 2. Add custom commands

Open the file in Visual Studio Code or your preferred text editor. Note that the dot we added before the filename creates a hidden file, so be sure you're able to locate and open it properly.

In the new file, add your custom commands using the following structure and save:

```bash
#!/bin/bash

function my_function_name() {
    python ~/path/to/my/script.py
}
```

## 3. Set up file permissions, if needed

The new file may generate a "permission denied" message. If so, you should be able to fix this by running the following command:

```sh
chmod +x .my_custom_commands.sh
```

## 4. Make it available in the terminal

If you try to run the command (the name of the function) you just created, you won't be able to quite yet. We'll need to let the terminal know to load your commands to each new session.

1. Open the `rc` file:

```sh
open ~/.zshrc
```

2. After the last line, add: 

```sh
source ~/.my_custom_commands.sh
```

3. Save the file, then exit and start a new terminal.

Once you have all this set up, you can add a new custom command any time by simply adding a new function to your commands file. Just note that you'll need to start in a new terminal session whenever you edit the file so your new command gets loaded up.

Aside from automations, this is also useful for repetitive strings of commands. Here's one I created to set up virtual environments for new Python projects, so rather than memorizing the extra commands I can just enter `create_env` and the rest is covered:

```bash
function create_env() {
    python -m venv env
    source env/bin/activate
}
```

As always, feel free to use this as a starting point and make it your own.

(Source: [Medium](https://medium.com/devnetwork/how-to-create-your-own-custom-terminal-commands-c5008782a78e))