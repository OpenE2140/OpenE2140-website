---
layout: post
title: "November 2026 release"
subtitle: "Development continues with incremental improvements"
author: "OpenE2140 developers"
date: 2026-11-22
summary: "New release improves Skirmish AI and adds quality-of-life improvements along with polishing and bug fixes"
published: true
---

It's been some time, since we've released new version of OpenE2140. This one is a smaller one (compared to some of the previous releases). It consists mainly from Skirmish AI (and other) improvements, gameplay features and a few bug fixes. Nevertheless, it's definitely worth to check it out.

Download links for the new version can be found on the [Download page]({% link download.html %}), release notes follow.

### AI can now build Water Base

AI players can finally build Water Base now and they're very capable at naval warfare:

<div class="mb-4 is-flex is-justify-items-center is-justify-content-center">
    <iframe title="OpenE2140: Naval battles with AI players" width="560" height="315"
            src="https://dalek.zone/videos/embed/iuUmnpKYqEGF2t7QqQyUjx" frameborder="0" allowfullscreen=""
            sandbox="allow-same-origin allow-scripts allow-popups allow-forms"></iframe>
</div>

Expect hectic battles at seas and shorelines.

### SDI Defense can now shoot down nukes

Community has called out several times, that SDI Defense has been a useless building (and didn't do anything at all) ever since it had been added. That changes now and it can destroy oncoming enemy nuclear missiles:

<div class="columns is-multiline is-centered">
    <div class="column is-4-desktop is-6-tablet">
        <video controls size="width: 100%" style="display: inline">
            <source src="{{ '/images/news/2026-11-22-sdi_defense_nuke_interception.mp4' | relative_url }}" type="video/mp4" />
        </video>
    </div>
</div>

### Quality-of-life improvements

Adding quality-of-life improvements is vital for OpenE2140. New version adds "atomic move + deploy" order for MCUs.

This feature is a big change, which is custom-made for OpenE2140 (not even OpenRA engine doesn't support it). Now you can make MCUs deploy at target location with single order - i.e. single click. Not only that, the UI shows overlays of any other MCUs moving to deploy somewhere.

This is opt-in feature (i.e. is **not enabled by default**); you need to **press and hold Ctrl key**. Direct deploy order is still possible via clicking on MCU, deploy button in command bar or hotkey. That way, you can choose, whether you want to use this feature or not. Take a look at how it works:

<div class="columns is-multiline is-centered">
    <div class="column is-4-desktop is-6-tablet" style="width: 36.1%">
        <video controls size="width: 100%" style="display: inline">
            <source src="{{ '/images/news/2026-11-22-mcu_deploy_heavy_tech.mp4' | relative_url }}" type="video/mp4" />
        </video>
    </div>

    <div class="column is-4-desktop is-6-tablet">
        <video controls size="width: 100%" style="display: inline">
            <source src="{{ '/images/news/2026-11-22-mcu_deploy_water_base.mp4' | relative_url }}" type="video/mp4" />
        </video>
    </div>
</div>

### New shell map

Shell map is the map, which is loaded at game start and runs in background of the main menu. Until now, we've used a simple one with small ED base and the only interesting thing going on were Banthas transporting resources crates back-and-forth.

This was pretty boring, so Dzierzan created a brand new shell map with plenty of action: two AI players battling out on the ground, in the air and on water. It's much more fun to watch what's happening on this map!

<div class="columns is-multiline is-centered">
    <div class="column is-4-desktop is-6-tablet">
        {% include image-card.html image='/images/news/2026-11-22-new_shellmap1.jpg' alt="New shellmap" %}
    </div>

    <div class="column is-4-desktop is-6-tablet">
        {% include image-card.html image='/images/news/2026-11-22-new_shellmap2.jpg' alt="New shellmap" %}
    </div>
</div>


### Other notable changes

One of the more visible changes is the addition of thruster trail that nuclear missile produces during its flight:

<div class="columns is-centered">
    <div class="column is-6">   
        {% include image-card.html image='/images/news/2026-11-22-nuclear-missile-thruster-trail.jpg' description="Nuclear missile finally looks like the one in Earth 2140." %}
    </div>
</div>

We've also fixed a few bugs in this release such as:
- Skirmish AI bots no longer build Refineries, where it would take Bantha too long to get there from Refineries (if they can build only Banthas)
- Newly produced unit shouldn't ignore rally paths (mainly affecting infantry)

Engine update brings these fixes/improvements:
- In Skirmish or MP lobby changing to certain map in certain situations shouldn't crash the game anymore
- Quicksave hotkey

Detailed list of changes can be found on the [GitHub's release page](https://github.com/OpenE2140/OpenE2140/releases/release-20261122).

### What's next?

Work will now continue with adding new gameplay features and improving existing ones. Stay tuned!

As always, for a high-level view of our current development plan can be found on [our roadmap]({% link roadmap.md %}) .

In the mean time, don't hesitate to join our [Discord server](https://discord.gg/KNcX5BxA37), where you can find and talk to other OpenE2140 fans and us developers. Occasionally, we post new bits of information on what we're currently working on. We're looking forward to see you there!
