---
author: "Daniell Mesquita"
title: "Since July Lots of News"
date: 2020-02-17T19:18:02-03:00
draft: true
tags: ["development", "logs"]
categories: ["logs"]
---

# Introduction

Since July of 2019, I'd stopped logging Floflis news on this blog. We moved from a room to a mini-kitchenet, the rent owner began reuniting with neighboors to contribute lawfare and personal harassment against us, and I could only focus on developing instead of also logging.


I know Floflis isn't just a home project. I'm not a professional developer. I'm more of a generalist girl with ideas for projects, not coding them like a robot.
Floflis, for me, isn't a idea for a test concept, but a need; a humanity tool which needs to be materialized.

# The background

First in 2007, year I had my first computer (a white computer with a fat monitor and a bluescreen-fan Windows 98, with a bluescreen accompained of creepy sounds), and despite my fear of computers after lots of Windows 98 issues, I also loved it and did my first draft of a OS. In 2008 I began a project of a paper computer, and did these concepts again in 2010 and 2011. But 2011 was special: I began the project of Plasma Development (originally, in portuguese, Plasma Desenvolvimento, which later become Plasmmer), ideas for Blogger-based services (and ironically, one of them worked as social network, even I being a newbie: Protestter, which used a Jotforms for posting and Blogger post-from-email, which worked like a pubsub made by a newbie at blogspot!) and started modifying my Windows, planning to create Windows Plasma.

# The struggles

In next years I knew SUSE Studio and for years planned to create PlasmaOS/Screens OS on it, but in 2018, when I came with all my forces to make it working, SUSE Studio was unusable. Thankfully, I've heard of Linux Respin programs, and like in 2011, began modifying my Ubuntu. That wasn't useful for creating my own OS (as then I'd discovered the respins programs aren't usable), but served as a huge experience leap. What comes next are the unlogged things that happened while developing Floflis, which wasn't yet in the blog till this post.


I know the above paragraph is confusing to read, but that truly represents my struggles in my journey of projecting a beaty, intuitive and purposeful OS to replace both Windows and Android. Floflis isn't simply a "let's spin my own distro with my own opinions". Floflis is backed by a common ideology and purpose.


From modifying and unsuccessfully trying to respin in a working Linux distro, I'd learned how to not-so-hardly create one directly in the ISO <3

# The simple and effective tools

## Shell/bash scripts

I didn't thought shell scripts (which I've heard in Windows universe as MS-DOS batch scripts) are so easy to program and so powerful ❤

Some skepticals told me I can't manage a entire OS from shell scripts; but I dare this challenge with all my love for democratic programming (that's why Eventoj, my if-this-do-that app creating program inspired by Construct 2/GDevelop will first kick start with shell). [Click here](/blog/2019/07/development-log-01-03-july-2019/) to read a post where I show all my love for 'sh' and explain how easy it is.

Floflis installer is very powerful yet simple bash script, and installers Floflis into different layers according to the user's needs. Other assistants and init services of Floflis are also shell scripts performing actions and managing its environment.

More will be covered at this post. Let's focus in the empowering tools which helped a newbie like me.

## SquashFS and ISO

I'd just discovered all major Linux distros (such as Ubuntu) ships compressed into a squashfs file, which is a OS filesystem, like a virtual machine, into a single file. Initially I thought programs/packages were .deb compressed, but what makes a ISO smaller is because the system itself is compressed. For experts it sounds like a obvious joke, but beginner OS enthusiats like me finds this amazing.

I've also heard of chroot, but just recently understand how it does exactly what I idealized. Chroot likely emulates a squashfs system in the terminal, and make you perform CLI actions just like if you were using this test OS live! Like I were doing on Windows in 2011 and on Linux in 2018-2019, but in a working approach.

Entering your squashfs OS you want to modify, you can do anything from its cmd. In my case, I could run Floflis Installer for it ( and apt didn't worked :/ - sorry, I'm writing from the dead Windows 7 and it doesn't haves emojis ) and modify the inner squashfs. Then, just deploy it to be inside a ISO, and it will live boot/install according to the packages I'd put on it and the modifications I did.

I came a whole decade to realize both 'sh' and SquashFS are the Harry Potter's sourcery magic recipes for developing a entire OS.

But there is a bonus:

## Rust programming language

Obviously, I'm not interested in learning how to program in Rust. I could create working JS scripts after a lot of struggles since 2014 (my Internet Cat browser relies purely in JS and works like a charm - for iframes hehe), but Rust requires you to do memory management. I don't even know what it is about. But as a generalist and intuitive at understanding the value of a project (like I hate ReactJS and love Mithril), I see a great potential in Rust as the next native language.

I always thought why not all programs/apps weren't written in JavaScript, for a unique codebase across Web, Mobile and Desktop. In 2016, the known project PokémonOnline.eu, laughed at my proposal. Pokémon Showdown also hatefully rejected. The obvious began to be considered by major enterprises, and despite Cordova being poorly used, Electron apps became a growing trend. Now, its practically a rule: all new desktop programs are wrapped into Electron framework. But I'm yet further on that: both Electron and Cordova should be united, and plus: native backing (does this word is used?).

Native backing, I mean, is a newbie like me programming in JS, and compiling to native language. That's were Rust also shone: WebAssembly loves it.

I could program in WebAssembly, which can be considered JS, and having my app running faster than the so-called native apps, by using Rust generated from WebAssembly.

How Rust will be fostered and used by Floflis, will also be covered by this post.

# The news since July 2019

## Floflis Installer is now Floflis CLI

It even gained its own site, at [floflis.github.io/cli](https://floflis.github.io/cli).

The main idea is Floflis CLI running as a backend, and Floflis Platform being the whole ecosystem concept.

## Where enters Floflis Platform

Like Google needing to create a parent company (Alphabet), Floflis became so complex it had the need of Floflis Platform to organize and categorize things. It's the ecosystem backing Floflis CLI, Internet Cat browser and HTML5Apps Platform (and futurely HumaneOS). Too much projects, I know; I'd never said I'm not crazy.

Now, Floflis Platform represents the whole Floflis' projects. Like Floflis Layers came to help at modularizing Floflis "core" (I hate monolithical things).

Floflis Platform is simply the main site of Floflis: [floflis.github.io](https://floflis.github.io) (should be IPFS instead of GitHub. Hugo will need a OmniLink extension for converting in Markdown files).

## A new direction for HTML5Apps Platform and Internet Cat browser

The new idea is, running one of them on your device, is likely running Floflis in a different form - it remembers Pokémon from 4th (or Deoxyes from previous)/5th generations.

Both will be part of a new project: Floflis Bridge, which will be backing in both CLI and visual (GUI). It means, the same magic which spawns IPFS on Internet Cat browser, also does it in HTML5Apps Platform, and also in Floflis for its updates.

## And HumaneOS borns

HumaneOS is inspired by MacOS, but this project will be postponned due to focus on Floflis underlying scheme. I won't tell much about it at this post.

Initially, HumaneOS was thought to be the distro manifestation of Floflis, while Floflis would be just a platform behind. But I've shifted it, and again Floflis will also be a distro (which is confusing by using the same name). But yes, I plan to fade Floflis as a distro with new approaches and names. HumaneOS? Screens OS, again? I should focus in other things first.

Because of that, a new project was created.

## First, Floflis-From-Scratch, before we introduce Declipse

Floflis-From-Scratch is about Floflis' dependencies which doesn't requires pegging into specific distro for that. It enables Floflis to pick its childs and move to new concepts.

Which is already part of that and will be easy to move, are: jq (CLI json manager), Hugo (static blog/site generator) and IPFS. It means Floflis can move from Debian to TinyCore, to BSD and redoxOS (and RISC-V based kernels) simply.

Here is the goddess of Floflis-From-Scratch:

## Floflis Declipse

The idea is the contrary of a eclipse: where Floflis splits its distro into different ones. It enables more modularity (like Floflis Layers and Floflis-From-Scratch) without depending on Debian and even Linux. Yes, actually Floflis depends upon antiX Linux (a modified Debian proudly not being corrupted by systemd's influence).
II'm a free thinker (without needing to be part of a Freemasonry for that) and I'm open to ditch Linux if something better is here. As I don't like the Bitcoin maximalists which even promotes Tron just to attack Ethereum.

Being open to move from Debian/Linux spectrum is a high jump against the conservatism of using macOS/Windows. If we get attached to Linux, we will be like Uber compared to taxi (as here is Arcade City, without the abusive taxes of Uber) and Windows users.

First, Floflis will move from antiX (whose developer is hateful and replied me with laziness and skeptism) to TinyCore (while fighting to fork Debian RISC-V without systemd), then to BSD (as a benchmark about how Floflis-From-Scratch can adapt), then a new step I didn't thought before and only recenly: redoxOS. Like a crazy, I'd searched if there is a OS or kernel entirely programmed from scratch in Rust. And there is! Moving to redoxOS is the longterm futuristic task of Floflis to show how Linux is becoming like Windows (like ARM doesn't differs from x86 - your raspberry pi isn't so open-source) and how archaic and weird this kernel is (as I'd said, I don't like monolhitic things, as web browsers shouldn't use a single thread). I love modularization, and redoxOS will be a big leap forward.

Also, as part of these migrating steps, Floflis' TinyCore version will have a custom Linux kernel called Librux (it's Linux, minus the proprietary libraries). It means less devices using the futuristic versions of Floflis; but isn't that the same for x64 and RISC-V? Also, in BSD phase, there will be a new project: Blunix, a mix between Linux and BSD. But first things first.

## Floflis Screens

Since 2013, I thought my OS project's UI should be in HTML5. I was pretty amazed when first met Firefox OS in 2014, and in 2015 began trying at modifying it (in the house of my uncle, and they deleted the files but a .html file with my name, they intentionally put inside the recyclebin - obvious it wasn't their idea, but external influences). Was sad when heard Firefox OS was discontinued in 2016, and happy when heard of KaiOS which could run on a 256MB-RAM feature phone). So, from my Screens OS idea, it spawns a new project: Floflis Screens. The work is creating a unique codebase UI for being used both in KaiOS and JADE (a Linux web Desktop Environment). The big milestone is this UI being compiled to native Rust using WebAssembly.

## Floflis Mobile

Not only Floflis Screens KaiOS-basis, but it could also have postmarketOS distros, Android ROMs and Floflis Installer supporting Termux.

## Floflis GSM

In december, I'd throw coffee at my old phone.
For much, that would be a step before gaining a new phone and a bless; for me, it is a bad thing in two sides. First, persons who are aiming me with lawfare will use it against, as a finance violence against mom. Second, I don't did it intentionally. But the thing is: I had the need to use GSM/3G modem instead of my phone's tethering. And: LINUX AND ITS F$CKN' DISTROS DOESN'T NATIVELY SUPPORTS THEM!

That's why I'd created the Floflis GSM project at floflis/meta git repo at GitHub. And it already had progress, with its base programs being installed by Floflis Installer (even with a GUI for managing and 'dialing').

## Floflis UDF

Even being futuristic, Floflis loves old things. Even being paradoxical, I think ditching old things is a retrocess. It means you have limited resources, to only focus in the present/future things instead of also supporting the registry value of the old.

Windows haves a amazing support for UDF discs (even it corrupting a few and not managing to fix it), while Linux focused more on flash drives; Windows, with large resources, could focus on both. And it have helped me a lot.

I'm fostering the creation of UDF 3.0, new usecases for optical discs and full UDF support at Floflis. Due to low resources, I can't focus too much on that yet. And its one of a lot reasons forcing me to yet rely on Windows for some things. I use UDF discs (they are not special, just standard CDs/DVDs/BDs formatted in UDF) because they are hard to tamper, and are the ideal storage media for blockchains, due to its read/append-only properties.

## Floflis Rust - yeah, Rust again <3

Part of Floflis-From-Scratch, is replacing in antiX (the Floflis' egg) a lot of programs to use purely-Rust alternatives.
Floflis is already open to replace its Terminal (which will be renamed to 'Sourcery', and the commands will be called 'magics'), replace git to Pijul, ditch bash/zsh to a Rust environment, and a lot others.

The shame here is I couldn't yet make Rust working, even rust-up saying it installed successfully.

## Other Floflis' projects

There are many projects for Floflis. It even had the need to split my floflis/meta git repo to the floflis/lab new repo.

I don't have a healthy mind now to cover all new projects. Autism haves a splendid flow in creating new things, but problematic at managing them.

## Floflis builds

It may be seem as lie, but Floflis did its first release. Not as a full blown OS/distro, but as its "core". Floflis CLI was launched to put Floflis inside Linux distros (turning them into Floflis OSes), with build 071 in July. Build 072 was launched as a update introducing the Layers (yes, it uses git for secure and fast updates). Floflis CLI with build 072 enabled Floflis DNA - ideal for wireless routers - being upgradeable to the next layer: Floflis Core. That's why I'd used quotes when I said "core" in this post: because Core is a layer, not to represent Floflis backend/CLI (like Soil is also a CLI layer). Also, Floflis Core, in build 072, installs jq (the json manager which will be ideal for managing things). For next update, and it is already done locally, Floflis Core also installs IPFS (and includes it on Floflis' own in-init system) and other programs.

Floflis have changed a lot. First, the idea was to create initial poor versions pegged to Floflis' nostalgy concepts since 2011, but now Floflis will just look forward (where I'm also preparing a blog post showing all the Floflis early concepts).

## Floflis in-init

It is a weird and novel system, using a bash script to manage Floflis while the system is booting. It even shows in the screen the Floflis' greeting. It is responsible for initializing IPFS daemon, and soon will also be used to manage updates - thankfully, not like systemd/Windows!)

The main idea of Floflis in-init isn't to being a init system. It is just a Floflis-exclusive tool for managing its initialization, with a fun name.

## New layers and changes on them

First, Floflis Quantum will now be called Planetary, for being shipped in Blurays. Quantum is a so big name for a layer which will not be compatible with so.

Then, there will be a new layer: Stellar, which will be for 1TB archival discs, which are the evolution of blurays. Hope our Internet (meshnets) gets so fast for downloading that.

And here comes Quantum layer (which jumped some layers), for 5TB discs and super powerful computers.

All Floflis graphical layers will come with gaming console emulators as a performance benchmark. Running 3DS games smoothly means you have a post-2010 computer. Those layers should be easy to update and manage.

## Less focus in NodeJS/Electron

The actual goal of Floflis is foundamenting in CLI, and native languages. Yes, Aragon (a DAOs framework) relies on NodeJS like Floflis' own developed apps, but shouldn't be the focus now. It will also help about Electron's security issues.

Also, here is a novel approach for HTML5 desktop apps: Muon, based in the WebKit fork Ultralight.

It also made the excellent decision to get rid of Dat protocol (which requires NodeJS) to only use IPFS (which comes with a single binary, very handy for Floflis-From-Scratch).

## New, novel licensing

Floflis is the first project to use OPI License, by Open Planet Initiative (also my project). Yet, OPI License is at initial stages of development and should be split into two different licenses: one for DAO-ownership, and other for more open projects.

Floflis, as a way to tackle on Windows/Micro$oft, will use OPI License stating Floflis pertains to Plasmmer DAO; it means its only for a few philosophical mens initiated in rites by me? Nope. You can contribute to Floflis (even without coding) and it will give you governance rights at both Floflis' and Plasmmer's DAOs. No priviledge for choosen persons by me, or staking by the richest. It's not only open governance but also the financing, empowering and openness of decentralized organizations to tackle in tiranies like Google and Facebook.

## Floflis Updates/IPFS Updater

Months ago I'd created a folder (and did 'git init') called ipfs-updater. It should be a modular core to not only be used by Floflis, but also other apps.

In Floflis' specific use case, every layer is its own git repo. Then, use a IPNS URL as a git remote for updating.

## Other news

A lot of news are undocumented. Too much for my head. But the majority are covered by this post.

Here is a quick list:

* CLI web-browser now is elinks
* Base layer will use Midori, Home will use Firefox, and Ultimate will use Brave (needs syncing between them and proper management, such as making Firefox available in Ultimate layer)
* Ultimate layer is a big evolution, as its decided it will be only for 64-bit system (but Floflis will not make the same error of Ubuntu, leaving Home layer and bellow yet supporting 32bit at its max)
* Brand new and special layer: Floflis Server
* Floflis Discs: Office, Coffee (a innovative office-parody, for programming/development), Media Center, etc). They aren't required to come at discs, and can simply be downloaded alongside or separatedly of Floflis
* Ditch the monolithic Cinnamon in prol of XFCE, but it will be a bad thing for user-pleasing, and changed mind again to use Cinnamon. Also, XFCE is pretty bad for GTK theming
* Fostering to implement GX (IPFS-based package manager), APM (Aragon's Package Manager), Cargo (Rust) and AppImage (developers insists in depending upon the f$ckng systemd)
* Stop the Linux polarization and splitting into different Linux distros and desktop environments; Floflis will implement common and synced settings between Cinnamon, XFCE, LXCE and KDE. Also, projecting a common system-events sound engine
* Other new things and achievements in Floflis Installer and the project as a whole

## Conclusion

No need to explain on this post how Floflis is important and taking a road no OS/distro had mind or courage to do. And that explains why Floflis is having a hateful backslash from conservatists (will be explained in the next post) and how Floflis is just one of other projects which makes me even more hated. No victimhood, it probably also happens to you if you're not enslaved in a job, is fair in not singing the same worldwide music of hipocrisy and is a fearless activist who thinks there isn't a limit on being militant, a limit imposed by the same power which permits and supports activism which seems to be challenging themselves, but just being part of their calming plans - Government-made UBI, industrial vegan-meat and homeless food foraging are examples of that).

Floflis is part of a lot reasons why they needs to arrest and kill me, but I'm already dead since I knew them (as I saw other people who, even accepting them, had deaths/loses from who they claims to love).

I'll keep fighting against nihilistic philosofies, existential crisis as a music to share, plain hate, bias, political/social polarization, hidden prosecutions, relativization of the truth and people's exploitation. That's the core mission of Floflis and its relatives.

The world is so manipulated (also with antenna's non-ionizing stimuling radiation), I only had desire to resume this post at day 17 (a number which makes evil persons crazy). It is being hard, slow, suffering, challenging, discouraging, threatning and being highly ignored and censored. Very before Floflis, manipulated persons were already looking me as a criminal and distorting things to point me as culprit of different things. But people shouldn't exist without a purpose; and majority of people thankfully borns being very different than the world's g-mens. Floflis will fight to bring happiness, which is basically why people keeps existing without the savage need of seeing the other's suffering. The world's top mens are so sad and psychopathic, that they needs the very intense experience of seeing their capital growing like in daily-trading profits, while poor persons needs very less than that to have a greater happiness. The Planet is dying. Freemasonry and politicans explains and claims but doesn't nothing more than inertia. Floflis is borning and living to change that.

> Post started at 19:18, done at 21:50.