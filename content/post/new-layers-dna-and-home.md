---
author: "Daniell Mesquita"
title: "New layers for Floflis: DNA and Home"
date: 2019-07-05T09:36:00-04:00
tags: ["development", "logs"]
categories: ["logs"]
---

I would post that on day 3, but had other things to do.
Thinking about Floflis powering routers (wireless), Core is a too much high layer.

# Floflis DNA

Then, Floflis DNA layer will get some things from Floflis Core (its installer, tree folder) while not having huge things such as NodeJS (making them optional to install; inside a router, possible to upgrade from DNA to Core).

# Floflis Home

Instead of upgrading from Floflis Basic (would work on Windows 95 machines) to Floflis Ultimate (heavyweight), it can have a middle stage for intermediate devices: Floflis Home.
So, this is the dependence scheme, including layers:

```
BIOS/UEFI
  -- Unix/Firmware
    -- Linux kernel
      --Floflis DNA
        -- Floflis Core
          -- BSD/GNU OS/Debian
            -- Floflis Substratum
              -- Cinnamon Desktop Environment
                -- Floflis Basic
                  -- Floflis Home
                    -- Floflis Ultimate
```

I'll write the complete and official guide about Layers on Floflis Documentation.

Read more about Floflis Layers [here](http://localhost:1313/blog/2019/07/floflis-layers-recipe-core-substratum-base-ultimate/).
