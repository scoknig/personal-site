---
title: "How to Automate Anything"
date: 2023-10-30T17:57:51-05:00
tags: [life, tech]
summary: My approach to automate the boring stuff and how you can do it too.
toc: false
draft: false
---

After some interest from my last post where I discussed some of my personal automations, I'd like to expand on the topic of personal automation a bit and discuss how you can automate (mostly) the boring or tedious stuff in *your* life!

I say "mostly" because while with enough time and resources, you *could* automate anything with a repeatable process. However, considering our main goal here is to save time, you'll have to evaluate which things are pragmatically worth expending your time and effort to automate.

Here's my general process:

## 1. Choose what you want to automate

An obvious first step, I know. But as I just mentioned, here's where you sift through your daily life to see where your pain points are. Make a short list of the most tedious things you'd rather not have to do, and then pick out the things that don't require human skill as part of the process. That is to say, the best candidates for automation are those with a repeatable process.

## 2. Record the steps

Now that you've chosen a task that can be reasonably automated, write out the steps to give yourself an idea of what the automation needs to accomplish. If the task is complex, that's okay for now. Just write down the general steps as a working outline.

## 3. Identify the most painful step

From the list you just created, look through the process to find the most pressing bottleneck or pain point. This is likely the best place to start automating. You may have thought we were going to automate the entire process all at once, but in my opinion it's best to start small and iterate your automation until it captures the overall process over time. 

This approach has several advantages:
- The effort of automating is minimized, since you are only tackling one *step* at a time.
- You get to test each step to make sure it works fully and accurately before moving onto the next.
- The work is spread out over time, so you don't spend one large chunk of time automating an entire complex process (unless you really, really want to).

## 4. Choose your platform

Now, for the task(s) you've just targeted for automation, you'll want to consider which platform best suits the triggers/actions involved. For example, my simple "Blog to Social Media" automation is done using [IFTTT](https://ifttt.com/) since there is no complex logic involved. That automation is simply a trigger (a new post is published to my [RSS Feed](https://scottk.mba/blog/index.xml)) and subsequent actions (a new post is published to Mastodon and X/Twitter) are executed.

A more complex example might be my financial automation. I'm taking a CSV of my checking account transactions, parsing through that and performing some matching to categorize each transaction, and then saving the result to an Excel file for my records. For this, I opted to write a custom Python script which handles the more sophisticated logic.

The point is, I choose a platform that's appropriate for the complexity level of the task at hand. It's not a one-size-fits-all sort of thing.

## 5. Automate it

You've chosen your most painful step to automate, as well as your platform. From here, create the script as required to solve the problem at hand. You may need to consider how often to run the automation or what triggers need to be configured so that the automation is run as needed.

Depending on the scenario, you might only need to run your automation manually (on a case-by-case basis, as my finance automation) or via some other action like my RSS-to-Social script.

As a tip: if you're opting for a no-code platform like IFTTT or Make to set things up, it still helps to have some surface-level familiarity with APIs and how to use them. This will come in handy for cases in which you need to interact with some service that doesn't have a built-in set of building blocks.

## 6. Repeat steps 3-5 until the whole process is automated

Keep working through your Step 3 list until the whole process is done. This will help you automate the most difficult parts of a process, significantly cutting down on your pain points even from the first iteration.

## 7. Deploy

Set up your automation using the appropriate triggers, as mentioned previously. If you're using an online service like IFTTT, this is probably already taken care of. If you've opted for something more custom like a Python script, you'll need to consider how to deploy that so it'll run when you need it. 

Good solutions for this could be [Netlify](https://www.netlify.com/), [Amazon Web Services](https://aws.amazon.com/console/), or one of any number of similar cloud hosting services. Find one that fits your expertise and budget.

## 8. Monitor, iterate, and improve

While this is all called "automation", you'd be sorely missing a step by just setting everything and forgetting about it. You'll want to monitor things over time to make sure that, once you're "done", everything *keeps* running as intended.

APIs and services change their available functions, the timing of tasks is prone to change at various points, and many other things may change over time from your initial configuration.

In addition, you may think of ways to improve your automation or use the extra time you've saved to add more steps that wouldn't have been possible when you were handling things manually.

Feel free to experiment, and have fun with it!