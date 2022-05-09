---
title: "HP Print Maker automated testing"
last_modified_at: 2022-04-30T11:50:00-08:00
categories:
  - HP
tags:
  - Testing
  - Software
  - Hardware
  - Automation
---

![{ site.url }]({{ site.url }}{{ site.baseurl }}/assets/images/print_maker.png)
While working as a Systems Interaction Engineer at HP my team was tasked with testing a new product, a small portable cube like printer now called the [Print Maker][print-maker]. This was pretty distant from what we were used to testing which was run of the mill home printers. Our testing for home printers was already very automated from software to communicate directly to the printer to test procedures that caused known failures to data collection. However, this product functioned entirely differently. Being literally driven by the user itself, this presented a challenge for testing.

## Solution
Another engineer on the team and myself decided that testing both could and should be automated to generate repeatable failures with distinct data. Our solution was to create 3d printed hardware that would hold the printer and could be easily assembled with parts that were always on site. To move the printer, we used a [Shapeoko CNC][shapeoko] due to its open source firmware and the ability to easily interface with custom software to drive it.

The software was written using three distinct abstraction layers. 1. The underlying layer that generates CNC code to move the printer and that communicates with the printer using a custom HP printer API. 2. A scripting layer that allow engineers to easily write tests without having to worry about printer position, talking with printer firmware, etc. 3. A GUI that would be used by techs to run the tests.

## Result
Overall the project was a success and allowed engineers to easily automate testing, especially testing that required exact time intervals. An example is testing how long the printer remains out of the cap and therefore determining whether ink drying would be an issue.


[print-maker]: https://www.linkedin.com/pulse/print-anything-anywhere-chad-q-martin/
[shapeoko] : https://carbide3d.com/shapeoko/
