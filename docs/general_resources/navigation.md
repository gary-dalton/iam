---
title: Navigation
subtitle: IAM
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

## Proposed

Embed waypoints into the field or along the path of the robot. Use the waypoints
to determine current location on a local map. Build the local map
manually, using the waypoints and a lightweight wheeled marker. The specific
details of the waypoints needs further research.
