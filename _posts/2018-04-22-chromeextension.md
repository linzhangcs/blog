---
title: Chrome Extension
subtitle:
date: 2018-04-22
author: Lin Zhang
layout: post
comments: true
img: noc/background.png
category: natureofcode
tags: [Nature of Code]
---
## Final Project Proposal: Gratitude forest

I am combining Nature of code's final with hacking the browser's. Here is a blog entry on the [project proposal](https://linzhangcs.github.io/blog/natureofcode/2018/04/15/gratitudeforest.html).

## Reverse Engineer - Gratitude Flow

As a part of my final project, I want to encourage chrome user to practice gratitude journaling. I searched the chrome store for extensions that similar. I want to reverse engineer an extension as a starting point. I found an extension called [Gratitude Flow](https://chrome.google.com/webstore/detail/gratitude-flow-happiness/bemnjoaibicimpimbigfmhoadacfaian), its message storing and sharing functionalities are some good entry points for what I want to do for my extension.

#### What permissions does it require?

It requires storage, alarms, unlimitedStorage, geolocation, and browser activity on https://*.gratitudeflow.io/*.

#### Does it have a browser action, page action, content script(s), background scripts, other?

Because this extension let users type in their thankful messages, save them, and share them. Multiple event scripts are included in the project, here is a screen capture of the scripts:
![background]({{site.baseurl}}/assets/img/noc/background.png)

The file structure of this project is well separated. So if anyone look into this project, he or she can identify which file to change for a certain functionality. Also there is something different about this project. Because it an extension that replaces the new tab page but not any other pages, it does not have content scripts.

#### What Chrome APIs does it use?

It uses the following Chrome APIs:
1. alarms - schedule code to run periodically or at a specified time in the future.
2. storage - store, retrieve, and track changes to user data.
3. permissions - request declared optional permissions at run time rather than install time, os users understand why the permissions are needed and grant only those that are necessary.
4. tabs - interact with the browser's tab system. You can use this API to create, modify, and rearrange tabs in the browser.
5. browserAction - put icons in the main Google Chrome toolbar to the right of the address bar. A browser action can have an icon, a tooltip, a badge, and a popup.
6. runtime - retrieve the background page, return details about the manifest, and listen for and respond to events in the extension lifecycle.
7. notifications -  create rich notifications using templates and show these notifications to users in the system tray.

#### In your own words, how does it work?

This extension works by replacing the default new tab page to main.html. This page is the interface page users see and interact with. The extension includes a lot of javascript based on events to store and retrieve user submitted messages.

#### What site(s) is it active on?

It is only active on the new tab page.

#### Find something else in the manifest, look it up in the manifest docs, and explain what it does.

Here are three lines in the manifest I did not know and looked up:
1. "background:{"persistent": false}"
2. "chrome_url_overrides": {
        "newtab": "main.html"
    }
3. "content_security_policy": "script-src 'self' https://ssl.google-analytics.com https://embed.doorbell.io https://api.survicate.com/assets/survicate.js ; object-src 'self'",

For number one, the persistent key makes event page rather than background page. The difference between the two seems to be event pages are loaded only needed.

For number two, chrome let developers substitute HTML files for default pages provided by chrome. An extension can replace bookmark manage, history, and new tab pages. Also an extension can override only one of those pages.

As for number three, this setting refers to the concept of [Content Security Policy](https://en.wikipedia.org/wiki/Content_Security_Policy). This setting works as a black/whitelisting for resources loaded or executed by extensions. Therefore, the setting above whitelisted the script source and object source from self and two urls.
