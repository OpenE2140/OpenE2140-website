---
layout: post
title: "Skirmish Alpha Release"
subtitle: "Skirmish AI is finally here."
author: "OpenE2140 developers"
date: 2026-08-30
summary: "After nine months of development, Skirmish AI is part of a new OpenE2140 release. Prepare for deadly battles with AI opponents!"
published: true
---

After more than nine months since development of Skirmish AI began, we're excited to announce that a basic Skirmish AI is now included in OpenE2140! Measure your battlefield skills against Easy, Medium, and Hard AI opponents—or, for those looking for the ultimate challenge, Cheating AI.

<div class="mb-4 is-flex is-justify-items-center is-justify-content-center">
    <iframe title="OpenE2140: Launch Trailer (Skirmish Alpha)" width="560" height="315"
            src="https://dalek.zone/videos/embed/b8G6Jg41ZbS8d8smyUY1tJ" frameborder="0" allowfullscreen=""
            sandbox="allow-same-origin allow-scripts allow-popups allow-forms"></iframe>
</div>


**TL;DR:** The latest version of OpenE2140 is available for download on the [Download page]({% link download.html %}). We strongly recommend reading the **release notes** and the other information below, or at least the **updated [list of known issues]({% link known-issues.md %})**. In addition to Skirmish AI, this release also brings more features, maps, improvements, and fixes.


### Skirmish Alpha

We're glad that our first release in November 2025, which focused on multiplayer, received positive feedback. However, many people were (and still are) interested mainly (or even solely) in **Skirmish** games against **AI opponents**. Therefore, we decided to shift our focus to Skirmish AI, which, even though it is far from complete, is a very formidable opponent in matches, whether it's against or alongside human players.

This release marks a historical moment in the long history of Earth 2140: it brings Skirmish and an Earth 2140-like RTS experience to players. Neither the original game nor the Mission Packs came with this feature. The closest thing is LAN multiplayer, which—as mentioned in our post about the Multiplayer Alpha release—was difficult to get working in the DOS version (and Windows versions didn't include it) and required at least one non-AI player anyway.

#### Current state

**Skirmish AI**, which comes with the newest release of OpenE2140, is currently in a very **playable state**. AI opponents know how to:

- Build, manage, and defend a base
- Expand their economy
- Research technologies
- Build armies
- Attack enemies
- Build and use superweapons

However, we recommend managing your expectations, because the way these activities are performed by the AI is far from perfect and still needs a lot of work. Some built-in engine bot modules will need to be replaced to make them work better in OpenE2140. We recommend reading the [article on Skirmish AI]({% link news/_posts/2026-01-18-basic-skirmish-ai-update.md %}) from January 2026, which provides a bit more description of what bot modules are and how the AI works in the OpenRA engine.

**Current limitations** and **known issues** of Skirmish AI include:

- Occasional planning issues with the deployment of MCUs
- Inefficient, erratic, and sometimes even illogical management of units, while attacking or defending
- AI keeps building weaker units, even if it can already build stronger ones
- Suboptimal placement of Refineries in relation to Mines

More in-depth information can be found on the [Known issues page]({% link known-issues.md %}).


#### Skirmish and multiplayer

After you've tried and experimented with playing local Skirmish games, we highly recommend playing multiplayer against AI opponents. OpenRA supports this well, and we've also tested it with our bot modules. A combination of AI and human players brings a whole new dimension to online games.


### Other changes

This new release packs in a lot of other things. Here's a list of the most important ones:

**12 new maps**

- Various types, including 1v1, 2v2, and more
- All created by Dzierzan

**Advanced submarine: *ORCA*** (new UCS naval unit)

- Counterpart to ED's KT-30
- Contributed by Narcoleptic

**Revamped DETECTOR** (UCS vehicle)

- New visual; now armed with dual machine guns
- Contributed by Narcoleptic

**Visual, UI, and other polishing:**

- Patches of player colors on ED defense towers and UCS Little/Big Eyes
- UI rendering issues with system screen scaling above 200%
- Missing beginnings and endings of smoke effects on damaged ships

**Improved random map generator:**

- Resources are now generated in patches, as in Earth 2140

**Gates**

- Useful for custom missions to make walled off areas accessible through gates

**Fixed gameplay bugs:**

- Water mine detection and targeting
- Aircraft couldn't attack other airborne aircraft with missiles
- "Stuck" Heavy Lifters when multiple ones tried to dock with a single Mine/Refinery

**Fixed rare crashes related to:**

- Heavy Lifters/Banthas
- Capturing buildings

... and the list continues. For the full changelog, see the GitHub release [release-20260830](https://github.com/OpenE2140/OpenE2140/releases/tag/release-20260830)

### Scenario map - Coastal Detour (2 Teams)

Since adding the ORCA submarine makes naval battles very interesting and fun, we wanted to give you an opportunity to try it out with Skirmish AI now. AI bots are not yet able to build Water Bases, so we came up with a solution to let you experience naval warfare in the meantime, until we teach the AI how to do it.

We created a variation of the Naval Warfare map called **Coastal Detour**. In this *scenario* map, there are four big bases already built and ready for you to start the battle! The map is supposed to be played in 2v2 teams, with each team composed of an ED and a UCS player. To quickly jump into battle, just add bots via **Slot Admin -> Add** (Configure Bots) and then pair yourself and the bots using **Slot Admin -> 2 Teams** (Configure Teams). You can also play with or against human players in multiplayer; just make sure to pick the correct slot and assign the correct teams, because the spawn points are fixed.

<div class="columns is-multiline is-centered">
    <div class="column is-4-desktop is-6-tablet">
        <video controls size="width: 100%" style="display: inline">
            <source src="/images/news/2026-08-30-coastal-detour-lobby.mp4" type="video/mp4" />
        </video>
    </div>
    <div class="column is-4-desktop is-6-tablet">
        <video controls size="width: 100%" style="display: inline">
            <source src="/images/news/2026-08-30-coastal-detour-gameplay.mp4" type="video/mp4" />
        </video>
    </div>
</div>


### Future plans

Skirmish AI remains our focus for the near future. Apart from fixing bugs in current features, we plan to add the ability to build Water Bases, thus unlocking full-blown naval warfare. Therefore, expect at least one more release with Skirmish AI improvements. There may be more, depending on whether there are any critical issues. After that, we'll transition back to implementing the remaining game mechanics, quality-of-life improvements, and polishing.

Check out [the roadmap]({% link roadmap.md %}) for a high-level view of our current work plan.

If you want to know more about the limitations of Skirmish AI and OpenE2140 in general, you can find more information on the [Known issues page]({% link known-issues.md %}).

### Getting in touch

Since Skirmish AI is now available in OpenE2140, we expect more people to try it out. We are happy to welcome everyone to our [Discord server](https://discord.gg/KNcX5BxA37), where you can talk to other OpenE2140 fans, connect with developers, get a sneak peek at development news, arrange multiplayer matches, and more!