---
title: "Temporal refinements and directional split refinements in project-level traffic forecasting"
categories:
  - Needs Review
---

Objective
=========

The objective of temporal refinement is to reduce the length of the forecast period, often from a 24-hour forecast to an hourly forecast, down to an interval that is more suitable for project-level evaluation. There are two ways of accomplishing this refinement: pre-assignment and post-assignment. Pre-assignment time-of-day factors must be applied within travel forecasting software, but post-assignment time-of-day factors may be applied after a travel model run has been completed. Time-of-day factors may also be used in adjusting traffic counts to a specific time period for an OD table estimation. Dynamic traffic assignments (DTAs) and traffic microsimulations may require O-D tables that are factored into time periods of less than one hour.

Directional split refinements are intended to improve upon directional splits from a regional travel forecasting model or to convert bidirectional volumes to directional volumes.

Background
==========

Many travel forecasting models are set up to provide forecasts for a full 24 hours or for multihour peak periods. However, projects are often evaluated by how well they perform over a single hour, either a design hour or a weekday peak hour. More than thirty years ago, time of day factors were published in NCHRP Report 255 (post-assignment) and NCHRP Report 187 (pre-assignment). The factors have been recently updated in NCHRP Report 765 (post-assignment) and NCHRP Report 716 (pre-assignment). Local factors are preferred to national defaults. Time-of-day factors can also be obtained from ITE’s “Trip Generation Manual”; these factors should be considered to apply post-assignment for site-specific traffic.

Default directional split factors are available from NCHRP 255, but these factors are old.

Guidelines
==========

The following guidelines relate to time-of-day factoring.

-   Locally derived factors are preferred over national defaults.
-   Factors derived from data for the specific highway being forecasted are preferred over data from nearby highways or from groups of highways having similar characteristics.
-   ADT forecasts may be converted to design hour forecasts using standard K factors for the Xth highest hour, if applicable.
-   Refer to software documentation for instructions on how to apply pre-assignment time-of-day factors.
-   Given the choice of both methods, pre-assignment time-of-day factoring is preferred over post-assignment time-of-day factoring.
-   Post-assignment time-of-day factors can be for any hour within a single day or for a design hour. These factors apply to vehicle trips at the time that they pass an individual street segment.
-   Post-assignment time-of-day factors are location specific and can vary by functional class, by location type (urban or rural), by urban area size, by day of week and by surrounding land use.
-   Pre-assignment time-of-day factors are broken-out by purpose and by direction of travel (to or from the trip production end). Totals of factors for a specific direction should be close to 0.5 or 50%, but they do not need to be exactly 50%. These factors apply to person trips but can vary by the type of vehicle; separate tables in NCHRP Report 716 give factors for “all modes”, “auto modes”, “transit modes”, and “nonmotorized modes”. These factors apply to trips at the time of departure at the origin end (either production end or attraction end, depending upon the direction of travel). Non-home-based factors can be assumed to be the same for both directions of travel.
-   Time-of-day tables should be inspected to assure that all the factors add to 1.0 or 100%, within a trip purpose.
-   When preparing O-D tables for short time periods or for a DTA application, 24-hour counts may be converted using post-assignment factors. However, counts that are adjusted in this manner should be given a smaller than usual weight in the O-D table estimation process.
-   NCHRP Report 765 describes a method whereby hourly time-of-day factors may be interpolated to periods of less than one hour, if necessary for DTAs. The method is given for pre-assignment factors, but the general idea will work for post-assignment factors, as well.
-   Time-of-day factors for trucks are different from time of day factors for automobiles. Example truck time-of-day factors can be found in NCHRP Report 765 and in FHWA’s original Quick Response Freight Manual from 1996. These factors should be considered to be post-assignment in their application.

Some states (e.g., Hawaii) do not maintain default K and D tables, preferring instead to develop those factors using historical data specific to a highway segment. The following steps may be used for development of post assignment time-of-day factors for individual highway segments having historical traffic count data, but are not continuous counting locations.

1.  Obtain weekday traffic counts by 15 minute intervals for the highway segment, in accordance with FHWA’s “Traffic Monitoring Guide”. 15-minute counts from each day of a 48-hour coverage count should be averaged together. It is recommended that counts be obtained for at least 5 separate prior years (but extending no more than 10 years in the past), if possible.
2.  Calculate the percent of daily traffic for each possible hour in the day, starting on a whole 15-minute interval for 15-minute counts. This should be done for each direction of a two-way highway. This will result in 96 hourly percentages for each day for a one-way highway and 192 hourly percentages for each day for a two-way highway. These percentages should be calculated to 3 digits past the decimal point, e.g., 8.325).
3.  Average these hourly percentages together across years, directionally (i.e., each direction separately) and bidirectionally (i.e., both directions together).
4.  The hour starting between 6:00 AM and 11:30 AM with the highest bidirectional average percentage shall be chosen to be the “AM peak hour”. The hour starting between 11:45 AM and 5:30 PM with the highest bidirectional average percentage shall be chosen to be the “PM peak hour”.
5.  The AM K factor is the average bidirectional percentage in the AM peak hour. Similarly, the PM K factor is the average bidirectional percentage in the PM peak hour. These factors shall be reported to the nearest tenth of one percent.
6.  The ratio of the directional factors or a single hour is the directional split for that hour. The directional split shall be reported to the nearest whole percentage for each direction of travel. The directional split is relative to a specific direction and should not be considered to be valid for both directions of travel.
7.  Compare the K factor values (time-of-day) to those from NCHRP Report 765 as a check for reasonableness.
8.  Compare the D factor values (directional split) to similar sites as a check for reasonableness.

Advice
======

Day-of-week factors may be useful in translating a forecast from a typical weekday to a specific weekday. However, day-of-week factors cannot be established with data from coverage counts. NCHRP Report 765 contains national default day-of-week factors. Day-of-week factors may also be used to convert weekday counts to a specific weekday, with caution.

Day-of-week factors (which are available in NCHRP Report 765) should not be used to convert weekday counts to a specific weekend day, unless there are no other options for obtaining weekend counts.

The growing interest in DTA suggests that in the future time-of-day factors should be computed in time increments of less than one hour, such as 15 minutes, from count data.

Items to Report
===============

-   Hourly factors
-   Hourly directional splits
-   Factored counts or factored volumes

References
==========

NCHRP Report 716 and NCHRP Report 765
ITE Trip Generation Manual
FHWA, Traffic Monitoring Guide
Quick Response Freight Manual, First Edition

