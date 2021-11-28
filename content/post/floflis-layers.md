---
author: "Daniell Mesquita"
title: Floflis' Layers (Recipe, Core, Substratum, Base, Ultimate)
date: 2019-07-01T16:44:03-04:00
tags: ["development", "logs"]
categories: ["logs"]
---

Seeing the need to compress files to make smaller .ISO file, and to run Floflis in other platforms (routers, IoT, handheld gaming consoles), I had the idea of Floflis' Layers, which makes Floflis modular and lightweight.

Bellow are the layers explained:

## Recipe

Not a working layer, but it contains references of compilers (for any supported platform) and source-codes.

## Core

Very lightweight, can run from a router to even a Nintendo DS. Focused on IoT devices. Totally based on CLI. Includes:

* Installer
* Directory scheme (tree, /1 folder)
* CLI web browser
* NodeJS
* Yggdrasil

## Substratum

Initially thought for Playstation 2. Contains a very basic UI (remembers Windows 1/3) that remembers a CLI, although can render some graphics.

* Dillo web browser
* IPFS
* Aragon + APM

## Base

A lightweight desktop version, thought to run on Windows NT/95 machines and above.

* Midori web browser (need to be compatible with Dillo browser)
* HTML5 apps (needs a lightweight webview that works on old devices)

## Ultimate

Contains all feature sets.

* Firefox web browser (need to be compatible with Midori browser)
* Application layers/loaders (Windows, MacOS, Android)
* Media softwares (video/audio edit, media player)
* others, from feature sets and packs

Actually, the first .ISO releases of Floflis will be from Base layer. With more knowledge, I'll create CLI tools to start distributing Floflis as Core, with ISO builds for other layers and possibility to upgrade a layer through ISOs or feature packs/sets.
