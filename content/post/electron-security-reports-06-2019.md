---
author: "Daniell Mesquita"
title: Electron security reports for Floflis' pre-installed apps
date: 2019-06-23T18:11:28-04:00
categories: ["security"]
tags: ["security", "reports"]
---

Some days ago I were studying about security auditors on Linux, firstly started with Electron apps auditing.

The first auditing tool (and currently the only I'm using) is Electronegativity by <a href="https://doyensec.com/" target="_blank">Doyensec</a>.

Electronegativity had pointed vulnerabilities in all apps. I don't know if they are really vulnerabilities or just JS best practices tips.

I've reported them to all developers, and they seemed skeptical, and ignored. But I'm committed to try to fix vulnerabilities in any app I develop for Floflis, specially its built-in apps. That is the reason I'll temporally remove `HTML5 Player`, as it is considered a web browser: which is the most sensitive kind of app.

Due to the bad <a href="https://github.com/fabiospampinato/noty/issues/10" target="_blank">responce received</a>, Floflis will remove `noty` as a installed app.

<a href="https://floflis.github.io/security/reports/06-2019/" target="_blank">Click here</a> for all reports, with link to their GitHub issue.
