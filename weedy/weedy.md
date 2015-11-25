---
title: Weedy
subtitle: IAM weedkiller bot
author: Gary Dalton
date: 24 November 2015
license: GNU General Public License, Version 2.0
github:
  user: gary-dalton
  repo: iam
  branch: "master"
framework: minimal
css: stylesheets/stylesheet.css
pandoc: pandoc -t html5 --standalone --section-divs --template=template_github.html index.md -o index.html
---

# IAM Weedy

## Concept

The Weedy concept is to remove weeds using methods that minimize environmental
impact. The market focus is for non-agricultural usage. Generally this means a
mowed lawn. Potentially this could be added onto a robotic mower.

## Status

Weedy is in very early stage development. This means gathering data,
reviewing literature, testing hypotheses, and building early concept-test
prototypes.

## Barriers

Many barriers to this concept exist. These include but are not limited to the
following:

1. low cost competition and infrastructure of herbicides
2. identification of weed versus grass
3. effective removal or destruction of weed
4. competition from established lawn care or mower businesses
5. robot navigation

### 1 Herbicides

More later

### 2 Weed identification

This is an obvious classification problem. A quick search determined that most
weed classification solutions have been developed with non-noisy background
The background has usually been soil which means that the weeds are not closely
mixed with other vegetation.

See the document weed_identification.md for additional discussion

### 3 Weed ablation

Once identified, the weed must be removed or destroyed such that it will not
return. Return may occur due to regrowth, new growth from seeds, or new growth
from parts. There are four main approaches to ablation that include: mechanical,
chemical, biological, or energy methods.

See the document weed_ablation.md for additional discussion.

### 4 Competition

Lawn care is a very large market with a wide variety of established players.

### 5 Navigation

The current generation of robotic mowers are not location aware but instead use
perimeter bouncing and random walk methods. **Perhaps this represents an
opportunity**.

See the document ../general_resources/navigation.md for further discussion.

## Links

- [Bosch's Giant Robot Can Punch Weeds to Death](http://spectrum.ieee.org/automaton/robotics/industrial-robots/bosch-deepfield-robotics-weed-control)
- [BoniRob – Robots](http://go.amazone.de/?lang=1&news=26)
- [Weed Detection Using Canopy Reflection](http://www.researchgate.net/publication/227215981_Weed_Detection_Using_Canopy_Reflection)
- [Discriminating Crop, Weeds and Soil Surface with a Terrestrial LIDAR Sensor](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3871132/)
- [Automation: The Future of Weed Control in Cropping Systems](https://books.google.com/books?id=yQ7IBAAAQBAJ&lpg=PA198&ots=ZoSQ9YmYxL&dq=wavelength%20reflection%20of%20weeds%20and%20grass&pg=PA200#v=onepage&q=wavelength%20reflection%20of%20weeds%20and%20grass&f=false)
- [DESIGN OF AN OPTICAL WEED SENSOR USINGPLANT SPECTRAL CHARACTERISTICS](http://www.ars.usda.gov/SP2UserFiles/Place/30200525/DesignOptical.pdf)
- [NIR and Vegetation – The Basics](http://flightriot.com/nir-and-vegetation/)
- [Precision Agriculture '09](https://books.google.com/books?id=aYEp6KPrUwMC&lpg=PA319&ots=HtvraajAJc&dq=wavelength%20reflection%20of%20weeds%20and%20grass&pg=PA319#v=onepage&q=wavelength%20reflection%20of%20weeds%20and%20grass&f=false)
- [How to install your Husqvarna Automower](http://www.husqvarna.com/us/lawn-and-garden/how-to-guides/automower-installation/)
- [Robomow](http://usa.robomow.com/shop/)
- [All Robotic Mowers Are Not the Same](https://www.probotics.com/robotic-lawn-mowers/robot-mower-compare.htm)
- [John Deere, Tango E5](https://www.deere.com/en_INT/products/equipment/autonomous_mower/tango_e5/tango_e5.page)
