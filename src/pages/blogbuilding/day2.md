---
layout: ../../layouts/MarkdownPostLayout.astro
title: "Day 2: Fixing Collections"
pubDate: 2025-Jan-24
description: "Well, I broke it"
author: "Anthony Larratt"
tags: ["astro", "blogging", "learning in public"]
---
## Where I Went

Today, like I expected, I broke collections. Well, kinda. When I stopped last time, I had just turned the existing post into a collection. With where I want to go, I decided to try to implement a new collection (this one) for documenting the building of this blog. To do this, I made a folder names "BuildingThisBog" with the markdown file "Day1.md" inside. I made adjustments to the content.config.ts file, as well as to the blog to switch my one collection from the posts folder to the BuildingThisBlog folder, aaaaand... it didn't work. I kept getting the mess of log files trying to load the Day1 post, so I restarted the dev server. This made it better, but was still getting a 404 error when trying to load the Day1 post. I did notice though, that the path was calling out day1, instead of Day1, so that got me thinking that this was a case sensitivity issue, and I was right. Changing the folder name to blogbuilding, and the post name to day1 (and making the appropriate changes in content.config.js and blog.astro), and the link worked!

Next was getting these changes sent up to show up here. VSCode made this easy. At least once I used git config to set my username and email.