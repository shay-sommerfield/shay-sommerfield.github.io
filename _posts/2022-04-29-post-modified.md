---
title: "HP Print Maker automated testing"
last_modified_at: 2021-03-09T16:20:02-05:00
categories:
  - HP
tags:
  - Testing
  - Software
  - Hardware
---


While working as a Systems Interation Engineer at HP my team was tasked with testing a new product, a small portable cube like printer. This was pretty distant from what we were used to testing which was run of the mill home printers. Our testing for home printers was already very automated from software to communicate directly to the printer to test procedures that caused known failures to data collection. However, this product functioned entirely differently. Being literally driven by the user itself, this presented a challenge for testing. 

Another engineer on the team and myself decided that testing both could and should be automated to generate repeateable failures with distinct data. Our solution 