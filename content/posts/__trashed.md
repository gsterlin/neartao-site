---
_last_editor_used_jetpack: block-editor
_publicize_done_22890294: "1"
_publicize_job_id: "86175889415"
_wp_desired_post_slug: ""
_wpas_done_24391465: "1"
author: neartao
categories:
  - uncategorized
date: "2023-07-29T19:05:48+00:00"
guid: https://neartao.com/?p=3962
parent_post_id: null
post_id: "3962"
publicize_tumblr_url: http://near-tao.tumblr.com/post/724207413896658944
timeline_notification: "1690658010"
title: Personal Project Management
url: /2023/07/29/__trashed/

---
Hey everybody!

I've been working through deciding what project management software to setup for myself personally, and I've been looking through several options. There's a lot of interesting paid software, open source software, and a lot of opinions of what is best to use, how they integrate together. It's a lot to dig through, but understanding others' experience with a tool is certainly helpful.

I've used Atlassian Jira, Redmine, Microsoft Project, Smartsheets, Bugzilla (though this was a freakish hack), text files, Cultured Code Things, Apple Reminders, and a boat load of other options.

## Requirements

Honestly, for my personal use I've got a few requirements, some of which I am learning conflict with each other.

- Free or single time license purchase
- Cross environment sync'ing
- Offline Access
- Home/on-premise deployment
- Multiple user accounts

About five years ago, I was definitely able to do this with several different solutions. Today though, I'm starting to find that the project management marketplace has moved in a different direction.

### Licensing

Let's start with the single time license purchase, because it is probably the most straightforward. I don't want to have to pay a monthly subscription, I already have enough of those. It's hard to get a clear and straight value out of it unless you use it all the time, and I'm not entirely sure that for my use case I'm going to get \*that\* much use out of it.

### Syncing

I'd like to have something that can sync projects and tasks across devices, such as my computer and my phone. This will allow me to work on projects where I am at. Some solutions don't seem to allow for this kind of workflow though, unless you're willing to setup email as a way to spam yourself with reminders. I'm on the fence on this one, but since I'm considering setting up a business and I would like a way to assign work to people beside myself, it would be nice.

### Offline Access

Besides syncing, which can sort of be done through cloud or online apps, I'd like to be able to get access to project details while I am not connected. It's tough when you have a network outage or don't have a good network connection to get access to information sometimes, and being able to work offline is nice.

### On-premise

This is a nit of mine, but I am getting tired of everybody having better access to my own data than me. Plus, I wanted to be able to get some more time putting into sys admin and deployments. Setting up my own instance seems like it has a lot of value to me for multiple reasons.

### Multiple Accounts

If I want to turn any of my work into a potential business, I'll likely need to hire people at some point. To be able to hire people you need to be able to assign them work. If a system doesn't allow multiple accounts, then you get stuck unable to assign work without a lot of copying and pasting.

## Atlassian Jira

I used to be a Jira admin, and was really considering setting this up at home. I was excited to see where things had progressed with Atlassian lately. Years ago, for a startup I had setup Jira and Bamboo, and had a really nice automated system running to allow for task creation, agile workflows, and it was all neatly integrated with Bamboo to run builds, and file bugs against builds. It took some work, but it generated a rich amount of reports and information. I had created a similar setup for things at home using a 10 person license, that I believe was $15 a month, for Jira, Confluence, and Bamboo. Sadly, the Bamboo license was more expensive to do anything terribly fancy with the builds, so I abandoned it.

At any rate, I still had my Atlassian account, and figured I would investigate pricing, and was surprised that their 10 user license was now free. Unfortunately, it is only free if you take their hosted SaaS solution, as they have discontinued their low cost licensed software. Maybe in the future I'll revisit using Jira, but for the time being I think I'll pass on it.

## Redmine

My first exposure to this was actually at my last job. When I started, there was no documentation, templates, or other efforts in place to help streamline work, and there was no budget to put anything into place either. I ended up taking the time to setup a Redmine server, create accounts, and get information deployed into it. I know it well enough that I didn't think it would be too hard to deploy, even if I wasn't terribly in love with the solution. Plus this was around ten years ago now, so it has probably grown up a lot.

My Synology used to have a Redmine option under Package Center, but it looks like this was removed somewhat recently. After doing a bit of research, it appears that it wasn't well maintained and was several versions out of date. I investigated deploying a container, but it looked like it was more trouble than it was worth. For the moment, I'll go with my instincts and just assume it isn't really what I am looking for and move on.

## MS Project

No thanks... and I'm not interested in MS Teams either.

## Things

I'd use this, because it checks off just about all of my boxes, but there's no multi user solution. It is purely a personal project/task manager. So for now it's actually just what I need, but for the future it's going to fall flat for me. I might have to give it some more thought depending on where other options land though.

## Reminders

This, or Notes from Apple might not be \*too\* bad in some ways, but it hits all the issues you're going to have with a text file. Lots of work to put up front to assign tasks, requires a lot of "agreements" between parties for how you want to manage it, and at the end of the day requires somebody to have an Apple device. So... probably not going to work the way I want it to.

## OpenProject

I did deploy this on my Synology in a container, and it was a bit janky, but I got it to work well enough. My broader concern though is that the majority of interesting workflows such as Kanban are locked behind an Enterprise subscription. Sorry, but I'm not interested in a subscription, and if I was I'd probably just go with Jira, since I know that software quite well.

## Kanboard

This is what I've ended up deploying as a container on my server. It is a bit simple, and missing some of the nicer flair of other options, but this is just project management. How much do you need? I'm going to play around with this for now and see how it works for me. If nothing else I'm pretty sure that I can go back to Things and see how it compares, but I do know that I need to get out of having all these sticky notes, text file docs, and other paper trails that are getting difficult to follow.

## Comparison

Just a quick chart for what I've noticed, and while it has a bunch of gaps, it definitely has shown me that I'm unlikely to find a single perfect solution.

SubscriptionSyncingOfflineOn-PremMulti UserJiraYes??????NoYesRedmineNo??????YesYesMS Project???????????????ThingsNoYesYesNoNoReminderNoYesYesNoYesOpenProjectYes??????YesYesKanboardNoNoNoYesYes

## Next Steps

For now, I think I'm going to play with Kanboard and see how well it works for me. I'll probably get some details written up on it in the future, especially if I learn anything interesting about it. There's certainly a lot of plugins, but as of today it does enough of what I want it to do, and I probably need to start working on setting up a build environment for my projects.
