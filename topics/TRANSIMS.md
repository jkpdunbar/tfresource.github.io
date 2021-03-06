---
title: "TRANSIMS"
categories:
  - Needs Review
  - Dynamic Network Models
---

Summary
-------

Dissatisfaction with the four-step modeling paradigm led David Albright, then director of research at the New Mexico DOT, to approach experts in the field of large-scale simulation at Los Alamos National Laboratory (LANL) in 1991. His challenge to them was to start from the requirements of the newly enacted ISTEA and Clean Air Act Amendments and to design, from first principles and without recourse to practices in use, a systems dynamics approach to modeling urban transportation systems. The resulting white paper, long since lost, formed the basis for a proposal to the DOE that eventually funded the TRANSIMS initiative.

The Los Alamos team made significant strides in the development of the population synthesizer ([Beckman et al. 1996](https://www.sciencedirect.com/science/article/pii/0965856496000043)) and began work on the route planner and traffic microsimulator. This was in contrast to the work of others, such as [Kitamura (1996)](http://media.tmiponline.org/clearinghouse/abtf/kitamura.pdf) and other early researchers in activity-based modeling, who focused on the demand side of the equation and largely ignored the supply side of the model. Regrettably, the two camps never collaborated to their strengths, largely as a result of the differences in opinion over how the overall framework would be structured or developed.

By early 1995, the LANL team implemented a cellular automata microsimulator and the distributed computer infrastructure (hardware and software) necessary to implement it. Tests on small prototype networks revealed promising emergent traffic flow properties ([Wagner et al. 1997](https://www.sciencedirect.com/science/article/pii/S0378437196003081?np=y)). The first TRANSIMS case study was carried out in partnership with the North Central Texas Council of Governments in 1996–1998. Because the activity generator had not been attempted, static demand from the Council’s regional travel model was sliced into small time intervals, from which trips and tour were synthesized. The entire Dallas–Fort Worth region was included in the model at a coarse level, with North Dallas being modeled in great detail. The [Dallas Case Study](Dallas_Case_Study) sought to prove the concept was viable, and the test was widely viewed as successful.

A second case study was launched in Portland, Oregon, in the spring of 2001. The goal was much more ambitious, including plans to model the entire region using the router and microsimulator and to commence work on the demand side (activity generator) of the model. Achieving the latter would result in operational modules for each part of the system. Extensive network development and testing was undertaken, with two network configurations compared. The development team had long thought that an "all roads" representation of the region was necessary, whereas others believed that the network used for traffic assignment from Portland Metro’s regional model would prove adequate. By late 2004, tests of both approaches led to the conclusion that the latter could effectively represent network conditions, although continued refinement of the network and testing of transit networks continued afterwards.

In 2005, the TRANSIMS team at LANL disbanded, having completed the work on the initial framework funded by internal sources, DOE funds, and limited USDOT support. The software was licensed as open source software a year later. During the same time AECOM undertook an extensive overhaul of several parts of the system to include porting the system to Microsoft Windows and improving the graphical user interface (GUI) and other user interaction components. Several more tests of the emerging system, carried out by academics in several locations, continued to add to the knowledge base about the model.

The open source implementation of TRANSIMS is the largest and perhaps the most successful such undertaking to date in transportation planning. FHWA decided on the desired outcomes, to include at the outset their long-term strategy for TRANSIMS and gradual transition to a user-supported community. The team made the decision to use an existing widely used open source license rather than writing one themselves. They also adopted common distribution strategies, making significant use of Internet technologies such as web pages, wiki pages, and accessible version control systems. The result is a vibrant, online, user community that is supporting several initiatives and projects. The [code repository](https://code.google.com/p/transims/) for the current version of the system is also accessible.

FHWA established an early deployment program in 2000 and continued to seek case study locations for the system. In contrast to the Dallas–Fort Worth and Portland case studies, most of the current deployments are for smaller studies. FHWA is also sponsoring research into the integration of TRANSIMS with activity-based travel demand models in Sacramento and Columbus.

------------------------------------------------------------------------

