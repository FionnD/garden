---
layout: post
title: Ditching Jira and using GitHub as our project managment tool 
truncated_preview: true
excerpt_separator: <!--more-->
---



There are probably few products that inspire such disdain as to have people create whole websites dedicated to the fact. For anyone who would consider contributing to [whyjirasucks.com,](https://whyjirasucks.com/) here is my experience of leaving Jira behind and embracing GitHub as our team’s project management tool. 

When I joined [Jina.ai](https://jina.ai/) our engineering team was composed of about 15 developers working in a typical scrum fashion. The first thing I noticed was the standard Jira vs real world chasm. Tasks would only be updated about 30 seconds before they were talked about in weekly meetings, the typical “Hey, quick reminder to all developers to update the status of tickets” Slack message populated the engineering channel. As a PM trying to onboard a new workstream, I was pretty pissed at the number of private messages I had to send asking for additional info or if a ticket was still valid or not. 

It got me thinking about how I could create a more organic project management setup, which would be accurate and therefore useful to someone looking into the project from the outside. 

Falling back on all those years in psychology lectures, I knew the process for developers to update the status of their tickets had to be as simple as humanly possible. Ideally automated. I considered using GitHub projects for this. I armed myself with three justifications when I pitched the switch to our product lead. 

1. Firstly, developers already have GitHub open and are using it daily. Therefore it should be easier for them to update tickets (reduce cognitive load). 
2. Secondly, we can add some degree of automation to move tickets automatically as pull requests are updated (reducing workload).
3. Thirdly, we are an open-source company, so our bug report primarily comes via GitHub issues. We no longer have to duplicate these into Jira to track them but can keep one source of truth inside GitHub.

Once the pitch was sold, I had to sit down and see how we could adapt GitHub projects to our day-to-day workflow. This coincided with us switching from scrum to kanban as a project management style. I believe using GitHub projects while the following scrum would be harder but not impossible. You’d have to create a board per sprint, labels per story point and have trouble moving the backlog but other than that I think it would be possible. 

Starting on the most basic level, each GitHub issue mirrored with what was previously a Jira ticket. They lived in our core code repository. Each issue was manually linked to a project board and placed in an appropriate column (backlog, in progress, in review, done). At the time of writing, GitHub did not support sub tickets, it now does. 

As mentioned previously, part of my pitch was we could employ automation to keep issues updated. Once a pull request was opened, every developer was required to link the PR to the appropriate ticket. Once the PR was merged, the ticket was automatically closed and moved to the done column. This also allowed developers to easily review pull requests by referring back to the original issue and user story when reviewing. 

To differentiate the type of issues we had (bug, feature request) we employed colour-coded labels. I strongly recommend reading sane [GitHub labeling by Dave Lunny](https://medium.com/@dave_lunny/sane-github-labels-c5d2e6004b63) which guided our approach on the matter. We followed a similar type, priority, size, area approach. 

### Now after six months of this GitHub madness, let me tell you how it went. 

Firstly, I believe our developers were happy. When anonymously surveyed on three occasions they reported 100% satisfaction rate with using GitHub as the project management tool. Not a huge sample size, and pretty company-specific but still a data point worth considering. 

Secondly, simply leaving Jira behind instantly gave me some kudos points with the engineering teams. I don’t think this is a great sign overall if i had stuck with the team long-term I probably would have moved them back to Jira at some point but regardless it was a quick win. 

From a personal PM perspective, I believe our project boards became considerably more accurate. At most an issue was one or two days out of sync compared with three weeks out of sync with Jira. 

On the other hand, one could rightly argue that the wins here are pretty personal and the benefit to the company (aside from the cost-saving of not using Jira) was pretty limited. 

As a team, I could have encouraged our developers to keep their issues more up to date. However, as a manager, I often believe you need to save your energy on the important battles, and I couldn’t see a valid reason to keep Jira in our current size. 

In summary, I would encourage PMs at smaller startup teams to not default to Jira. There are similar (and cheaper) tools out there that in my experience work just as fine. 




![3a4bzppsi8y41](https://user-images.githubusercontent.com/59612379/138683391-8a05d7bb-d493-45a6-a1c9-d357af0841ea.jpeg)










