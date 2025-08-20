---
title: "Updates from June 2025"
date: 2025-07-07T05:01:14
slug: "updates-from-june-2025"
tags:
  - freebird
---

# Updates from June 2025

*Note: Freebird is free for students! If you're a student at a school or college, please feel free to [email](mailto:dev@freebirdxr.com) or [message me](https://discord.gg/X6B4ZYEWSS) for a free copy!*

June 2025 marked a restart of the Freebird project, after a few months of maintenance-only fixes.

## Reliability

My focus in June was on improving Freebird's reliability. A number of long-standing critical bugs have been fixed, broken features have been repaired, and missing documentation has been updated. Basically, anything that crashed Freebird (or was urgently broken) was considered as an immediate priority.

I'm still investigating a Blender crash (that happens occasionally). So please save your work frequently.

I'm sure Freebird still has undetected bugs, so please let me know on [#support](https://discord.gg/jvHsCPzHBN) if Freebird crashes for you. But a number of those crashes were fixed in June, and a focused effort has been made to improve the reliability.

## Features

In terms of features, [Free Extrude](https://freebirdxr.com/docs/edit/extrude/) is back, and the [transform gizmos](https://freebirdxr.com/docs/transform/#moverotateresize-along-specific-axes) now support moving/rotating/resize along specific planes. The transform gizmos now also support mode-specific transforms, i.e. the ability to move without rotating/resizing, rotate without moving/resizing, or resize without moving/rotating.

## Tools to help improve reliability

To help investigate difficult-to-recreate bugs, I added an event record/replay developer tool in Freebird. If Freebird crashes at any point while running (on my PC), I can replay those exact button presses and movements any number of times, and check Freebird's code while running it. I've fixed a few difficult-to-recreate bugs using this tool. Note: This tool is disabled by default for users, so Freebird isn't recording your actions.

Another improvement was to run Freebird's automated tests in a random order, using [pytest-random-order](https://pypi.org/project/pytest-random-order/). Freebird already runs over 600 automated tests (which check various aspects of Freebird before a new version is released). But those tests used to run in a fixed order previously. Since I can't predict the order in which a user will use Freebird's tools, I'm now running the tests in a random order. This helps ensure that Freebird is reliable regardless of the order in which you use the various tools. This change has already revealed a couple of hidden bugs (that have been fixed).

## Community
The [Discord community](https://discord.gg/X6B4ZYEWSS) has grown to nearly 1200 members, and it is active at trying out new [Early-Access](https://freebirdxr.com/docs/early-access/) features and providing valuable feedback!

Some user experiments using Freebird:

* [Celso Teixeira's review and workflow tips](https://www.youtube.com/watch?v=V7xz6M1y8qA)
* [Matt Estela's experiment](https://discord.com/channels/993812566298083390/1038282345645609060/1347292653229838366)
* [Oliver Döhring's experiment](https://discord.com/channels/993812566298083390/1038282345645609060/1336762370214596789)
* [YENO's experiment](https://discord.com/channels/993812566298083390/1038282345645609060/1314193069595430942) and [another](https://discord.com/channels/993812566298083390/1038282345645609060/1320899960929259634)
* [ilovebridge's experiment](https://discord.com/channels/993812566298083390/1038282345645609060/1378917855772278854)

Did I miss any? Please send me your cool "made with Freebird" videos!

## Next

Lots more to come. The focus, as always, remains on making VR a part of your daily design workflow.

Thanks!

[Get started with Freebird!](https://freebirdxr.com/getting-started/){ .md-button }