# Frequently Asked Questions regarding Google Earth Engine (GEE)
*last updated: 27.04.2026*

## Disclaimer
*The perspectives expressed here **do not** represent those of Google or my employer.*

## Objective
This document is intended to provide the general public - and particular novice users of Google Earth Engine - with general information about GEE.

## Questions

* How does GEE compare to a desktop GIS software program like *ArcGIS Pro* or *QGIS*?
* When would someone use GEE vs. a desktop GIS software program (e.g., ArcGIS Pro, QGIS), and vice versa?
* Is it true that Google is now charging for GEE use?
* Can someone explain the various changes to GEE's overall terms of service?
* Can you lay out the various recent milestones regarding GEE's terms of service changes?

## GEE Terms of Service milestones
* **28 June 2022**: Google announced non-commercial and commercial tiers via the [Introducing Earth Engine for governments and businesses](https://blog.google/products-and-platforms/products/earth/introducing-earth-engine-for-governments-and-businesses/) article.
  * With this change, Google also introduced Earth Engine compute use (EECU) estimates visible for batch processing. The initial announcement also provided [pricing information](https://cloud.google.com/earth-engine/pricing) for EECUs (initially US $1.33 / EECU-hour per month for online usage, and $0.40 / EECU-hour per month for batch processing, *later* revised to only $0.40 / EECU-hour for the first 10,000 hours, and $0.28 / EECU-hour for 10,000 hours to 500,000 hours, and $0.16 / EECU-hour for usage exceeding 500,000 hours in a month).
  * Through this update to GEE's terms of service, GEE opened the possibility for [businesses and governments](https://blog.google/products-and-platforms/products/earth/introducing-earth-engine-for-governments-and-businesses/) to begin paying for their GEE use, while also affirming free use of GEE for non-commercial purposes. Business use of GEE was defined as "commercial," while government use of GEE was characterized as "operational."
* **24 July 2024**: Google announced that entry to GEE would be facilitated via Google Cloud projects; this was summarized in the following Google Developers page entitled ["Transition to Cloud projects for your workflows"](https://developers.google.com/earth-engine/guides/transition_to_cloud_projects).
  * Previously, GEE users did not need Google Cloud projects to access GEE. This condition particularly affected US university and institutional users, since many US universities and institutions restrict the creation of Google Cloud projects. A work-around was that such projects could be created using users' Gmail addresses, and their university / institutional email addresses could be added to those projects. As it turns out, many GEE users have multiple GEE accounts (e.g., through their personal Gmail addresses and through their work email addresses).
  * That said, there was some confusion, with some users / institutions erroneously perceiving this change to access as Google removing access to GEE.
  * In addition to setting up Google Cloud projects, users also had to be document how those Cloud projects matched commercial or non-commercial goals.
* **20 Jan. 2026**: Google announced restrictions on their non-commercial tiers, summarized in the [Earth Engine Noncommercial Tiers](https://developers.google.com/earth-engine/guides/noncommercial_tiers) page.
  * Previously, GEE users had access to unlimited computational resources via GEE. With this change, Google effectively started *significantly* throttling the quantity of compute that GEE users can access.
  * That throttling became effective on 27 April 2026.
  * Three tiers of use were created: (i) Community (with access to up to only 150 EECU-hours / month), (ii) Contributor (with access to up to only 1,000 EECU-hours / month, but requiring a Google billing account), and (iii) Partner (with access to up to 100,000 EECU-hours / month).

## GEE non-commercial quota limits (*as of 27 April 2026*)
[*source*](https://developers.google.com/earth-engine/guides/noncommercial_tiers): Google

**Table x.** GEE non-commercial tier limits

| Tier | EECU-hour limits | EECU-second limits | Approx. value (US) |
| --- | --- | --- | --- |
| 1. Community | 150 | 540,000  | $60 |
| 2. Contributor | 1,000 | 3,600,000 | $400 |
| 3. Partner | 100,000 | 360,000,000 | $40,000 |
