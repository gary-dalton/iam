---
title: Navigation
subtitle: Intellamech
author: Gary Dalton
date: 25 November 2015
license: GNU General Public License, Version 2.0
github:
  user: gary-dalton
  repo: iam
  branch: "master"
framework: minimal
css: stylesheets/stylesheet.css
pandoc: pandoc -t html5 --standalone --section-divs --template=template_github.html index.md -o index.html
---

# Navigation

Intelligent robots should be at least somewhat location aware. Perimeter
bouncing indicates the robot is blind until it meets a certain condition.
Perimeter bouncing is a valid strategy to building an initial local map but
should not otherwise be considered a valid navigation method.

## Real Time Location Services

There are many RTLS in operation, mainly using RFID, BlueTooth, WiFi or GPS
technologies. All but GPS are relatively ineffective in an outdoor weather
impeded environment. GPS has the disadvantage of loss of signal and low
distance resolution.

There are two other technologies that are not in high use but may have
significant advantages. These are Ultra Wideband (UWB) and [VHF Omni
Directional Radio Range (VOR)](https://en.wikipedia.org/wiki/VHF_omnidirectional_range).
VOR is an aviation navigation aid and likely would not be permitted for RTLS.
Alternatively, UWB is included in the [IEEE802.15.4-2011 standard](http://www.decawave.com/technology/ieee802154a-standard). UWB is also
considered to provide data services.

See [rtls.md](rtls.md) for more info.

## Proposed

Embed transceivers into the field or along the path of the robot. Use the
transceivers to determine current location on a local map. Build the local map
manually, using the transceivers and a lightweight wheeled marker. The specific
details of the transceivers needs further research.
