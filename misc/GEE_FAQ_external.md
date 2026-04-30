# Frequently Asked Questions regarding Google Earth Engine (GEE)
*last updated: 30.04.2026*

## Disclaimer
*The perspectives expressed here **do not** represent those of Google or my employer.*

## Objective
This document is intended to provide the general public - and particular novice users of Google Earth Engine - with general information about GEE, as well as its potential relationships with desktop Geographic Information Systems (GIS) software programs like ArcGIS or QGIS.

## Questions

* **How does GEE compare to desktop GIS software programs like *ArcGIS Pro* or *QGIS*?**
  * **Overall:** One may consider the difference between a **cloud-based** platform like GEE and a **desktop** program like ArcGIS or QGIS to be like the difference between a fork and a spoon. That is, they can be seen as serving different functions. Geospatial operations have long been described in terms of (i) vector-based operations, and (ii) raster-based operations.
  * **Raster analysis:** GEE excels in raster-based operations, and can be considered as a cloud-based version of ArcGIS' *Raster Calculator* feature.
  * **Vector analysis:** On the other hand, ArcGIS and QGIS are generally seen as much more adept than GEE in handling vector-based operations, with GEE generally tending to throw errors for complex geometrical features which possess many vertices.
  * **Cartography:** The general consensus is also that for the cartographic side of geospatial operations (i.e., map-making), ArcGIS and QGIS are better suited to generating attractive and customizable map layouts than GEE, for which generating apps or screenshots are the main options for map-making.

* **For my general information, how do ArcGIS and QGIS compare?**
  * **Cost:** The main differenciator between ArcGIS and QGIS is cost. ArcGIS is a [paid] commercial off the shelf software, and QGIS is an open source [**freeware**](https://en.wikipedia.org/wiki/Freeware) software package.
  * **OS compatibility:** Another significant difference between ArcGIS and QGIS is that ArcGIS cannot be run in the macOS operating system, largely limiting ArcGIS' use to computers running Microsoft Windows. Hence, it would seem that QGIS would be the software of preference for Apple users. That said, according to the QGIS [monitoring dashboard](https://feed.qgis.org/metabase/public/dashboard/df81071d-4c75-45b8-a698-97b8649d7228), of over 761 million QGIS instances opened over the previous 30 days (*as of the morning of 30.04.2026*), only 2.95% have been on macOS, compared to 64.7% on Windows, and 0.29% on Linux (with an addition 30.7% on unreported operating systems).

<img width="290" height="243" alt="image" src="https://github.com/user-attachments/assets/8f8fec0b-a929-412f-9e29-6316599a1176" />

* **How can I get access *right now* to GEE, ArcGIS, or QGIS?**
  * **GEE:** Since GEE is a Web-based platform, one registers for access via https://earthengine.google.com/signup/, and one can thereafter access the GEE Code Editor via https://code.earthengine.google.com. Since late 2024, Google has also required that users access GEE via Google Cloud projects. Instructions on how to do so can be found at: https://github.com/BzGEO/GEE_resources.
  * **ArcGIS:** Procuring an ArcGIS Pro license can be a little challenging, especially since access is usually through organizations registered with Esri. More information can be found here: https://pro.arcgis.com/en/pro-app/latest/get-started/download-arcgis-pro.htm. In addition to institutional level ArcGIS Pro access, Esri also offers an **ArcGIS for Personal Use** option, via: https://www.esri.com/en-us/arcgis/products/arcgis-for-personal-use/buy. *ArcGIS for Personal Use* is sold as a subscription-based service, which in the USA costs US $100 / year.
  * **QGIS:** You can download QGIS at no cost from: https://qgis.org/download/.

* **When would someone use GEE vs. a desktop GIS software program (e.g., ArcGIS Pro, QGIS), and vice versa?**
  * **Scenario:** You need to do **intensive vector-based analyses** on shapefiles (e.g. clipping, erasing, merging, unions, etc.) ➡️ Use ArcGIS or QGIS
  * **Scenario:** You want to do **basic analysis of satellite data** and you want to have the peace of mind of having the data stored on your computer ➡️ Use ArcGIS or QGIS
  * **Scenario:** You need to **compare vegetation indices across multiple satellite platforms** (e.g., ASTER, GOES, Landsat, MODIS, Sentinel-2, Sentinel-3, VIIRS) ➡️ Use GEE
  * **Scenario:** You want to do a ***land cover classification*** of Landsat or Sentinel-2 imagery for a fairly small area (one or a few tiles) for which you (i) don't mind downloading data and (ii) don't mind how long it might take for the classification to run on your desktop or laptop computer ➡️ Use ArcGIS or QGIS
  * **Scenario:** You want to do a ***land cover classification*** of Landsat or Sentinel-2 imagery for a large area (many tiles), and for which you (i) don't want to or have the time to download data and (ii) you don't want to wait hours to do image preprocessing and for the classification to run ➡️ Use GEE
  * **Scenario:** You want to do a ***land cover classification*** of Landsat or Sentinel-2 imagery, iteratively, so you need to run the classification dozens of times to see what works ➡️ Use GEE
  * **Scenario:** You need to extract ***spectral signatures*** from openly accessible hyperspectral data like EO-1 Hyperion or EMIT, you don't have access to specialized software like ENVI, and you don't have time to download all the available hyperspectral scenes for your area of interest ➡️ Use GEE
  * **Scenario:** You need to do a ***time-series analysis*** of changes in NDVI (e.g., using Landsat, Sentinel-2, MODIS, VIIRS), over a large period of time, and you don't have the time to download large quantities of data ➡️ Use GEE
  * **Scenario:** You need to do **zonal statistical analysis** on multiple satellite images (e.g., Landsat, Sentinel-1, Sentinel-2, Sentinel-3, MODIS, VIIRS), and you don't want to download the data ➡️ Use GEE
  * **Scenario:** You need to do **zonal statistical analysis** on a very large (e.g., continental) scale ➡️ Use GEE
  * **Scenario:** You want to **generate a nice map** and customize the layout ➡️ Use ArcGIS or QGIS

* **How does GEE compare to ArcGIS and QGIS in terms of their respective user bases?**
  * **GEE:** At Google's *Geo For Good* 2025 conferences (in [August](https://earthoutreachonair.withgoogle.com/events/geoforgood25-nyc), [September](https://earthoutreachonair.withgoogle.com/events/geoforgood25-singapore) 2025), it was indicated that there are **over 100,000 monthly active users** of the platform.
  * **ArcGIS:** According to the Esri [Wikipedia page](https://en.wikipedia.org/wiki/Esri), ArcGIS has **over a million active users** (*date unknown*). Esri's overview [page](https://www.esri.com/en-us/about/about-esri/overview) indicates that its products (presumably ArcGIS) are used by 33,000 businesses, 1,200 national government agencies, 30,000 cities and local governments, and 12,200 nonprofit organizations.
  * **QGIS:** According to a Dec. 2023 *Medium* [blog post](https://gispofinland.medium.com/how-big-is-the-qgis-community-now-b20978ea7eac) by GISPO Finland Ltd, in May 2023, QGIS was opened 13,629,896 times. GISPO developed a [dashboard](https://feed.qgis.org/metabase/public/dashboard/df81071d-4c75-45b8-a698-97b8649d7228) for tracking QGIS use, which indicates that QGIS was **opened 21,903,891 times in the last 30 days** (*as of the morning of 30.04.2026*).
    * The dashboard estimates that there are only 26 QGIS users in Belize, compared to 1.08 million users in Guatemala, 284 users in Panama, 40.55 million users in Brazil, 19.4 million users in the USA, 45.3 million users in France, and 35.2 million users in India. In fact, the dashboard indicates that *on 29.04.2026*, the major uses of QGIS were in the following countries (in descending order): Brazil, Germany, France, India, Spain, Italy, Indonesia, the USA, Poland, and Mexico.

<img width="776" height="464" alt="image" src="https://github.com/user-attachments/assets/673aebac-102f-46a7-a24c-2b8601b6a4f9" />

* **Is it true that Google is *now* charging for GEE use?**
  * GEE launched in Dec. 2010 at the UNFCCC Conference of the Parties in Cancun, Mexico. It was not until June 2022, however, that Google announced via a [Google Blog post](https://blog.google/products-and-platforms/products/earth/introducing-earth-engine-for-governments-and-businesses/) [*Terms of Service*](https://earthengine.google.com/noncommercial/) which established various categories of use, "*So starting today, we’re making Google Earth Engine available to businesses and governments worldwide as an enterprise-grade service through Google Cloud.*"
  * Those categories can largely be distinguished between commercial and non-commercial uses. For details on each category (shown in the screenshot below), see: https://earthengine.google.com/noncommercial/

<img width="399.3" height="216.48" alt="image" src="https://github.com/user-attachments/assets/e0b035db-07e5-46c1-954d-094a755c75ab" />

* **Can someone explain the various changes to GEE's overall terms of service?**
  * Please refer to the section below on the milestones regarding GEE.

## GEE Terms of Service milestones
* **28 June 2022**: Google announced non-commercial and commercial tiers via the [Introducing Earth Engine for governments and businesses](https://blog.google/products-and-platforms/products/earth/introducing-earth-engine-for-governments-and-businesses/) article.
  * With this change, Google also introduced Earth Engine compute use (EECU) estimates visible for batch processing. The initial announcement also provided [pricing information](https://cloud.google.com/earth-engine/pricing) for EECUs (initially US $1.33 / EECU-hour per month for online usage, and $0.40 / EECU-hour per month for batch processing, *later* revised to only $0.40 / EECU-hour for the first 10,000 hours, and $0.28 / EECU-hour for 10,000 hours to 500,000 hours, and $0.16 / EECU-hour for usage exceeding 500,000 hours in a month).
  * Through this update to GEE's terms of service, GEE opened the possibility for [businesses and governments](https://blog.google/products-and-platforms/products/earth/introducing-earth-engine-for-governments-and-businesses/) to begin paying for their GEE use, while also affirming free use of GEE for non-commercial purposes. Business use of GEE was defined as "commercial," while most government use of GEE was characterized as "operational."
* **24 July 2024**: Google announced that entry to GEE would be facilitated via Google Cloud projects; this was summarized in the following Google Developers page entitled ["Transition to Cloud projects for your workflows"](https://developers.google.com/earth-engine/guides/transition_to_cloud_projects).
  * Previously, GEE users did not need Google Cloud projects to access GEE. This condition particularly affected US university and institutional users, since many US universities and institutions restrict the creation of Google Cloud projects. A work-around was that such projects could be created using users' Gmail addresses, and their university / institutional email addresses could be added to those projects. As it turns out, many GEE users have multiple GEE accounts (e.g., through their personal Gmail addresses and through their work email addresses).
  * That said, there was some confusion, with some users / institutions erroneously perceiving this change to access as Google removing access to GEE.
  * In addition to setting up Google Cloud projects, users also had to be document how those Cloud projects matched commercial or non-commercial goals.
* **20 Jan. 2026**: Google announced restrictions on their non-commercial tiers, summarized in the [Earth Engine Noncommercial Tiers](https://developers.google.com/earth-engine/guides/noncommercial_tiers) page.
  * Previously, GEE users had access to unlimited computational resources via GEE. With this change, Google effectively started *significantly* throttling the quantity of compute that GEE users can access.
  * That throttling became effective on 27 April 2026.
  * Three tiers of use were created: (i) Community (with access to up to only 150 EECU-hours / month), (ii) Contributor (with access to up to only 1,000 EECU-hours / month, but requiring a Google billing account), and (iii) Partner (with access to up to 100,000 EECU-hours / month).
* **TL;DR**: In 2022, Google changed their Terms of Service for GEE, defining commercial vs. non-commercial uses, with commercial uses being those for which Google should be paid for GEE use.

## GEE non-commercial quota limits (*as of 27 April 2026*)
[*source*](https://developers.google.com/earth-engine/guides/noncommercial_tiers): Google

**Table 1.** GEE non-commercial EECU tier limits

| Tier | EECU-hour limits | EECU-second limits | Approx. value (US) |
| --- | --- | --- | --- |
| 1. Community | 150 | 540,000  | $60 |
| 2. Contributor | 1,000 | 3,600,000 | $400 |
| 3. Partner | 100,000 | 360,000,000 | $40,000 |
