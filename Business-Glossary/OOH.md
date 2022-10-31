---
title: OOH
description: 
published: true
date: 2022-10-18T14:49:49.420Z
tags: 
editor: undefined
dateCreated: 2022-10-18T14:25:25.307Z
---

# Glossary

![ooh_1.png](/ooh/ooh_1.png)

![ooh_2.png](/ooh/ooh_2.png)


**POI CLASSIFICATION:**
**POI**: Point of interest, based on number of facilities, population, and number of hexes
From **2020 CACI data**, considered relevant POI features to classify zips into high, medium, and low basis POI presence. Considered number of hexagons in each zip to account for zip area.
Each POI feature is categorized across ranges and assigned scores
For each zip, the total score is aggregated across the **8 weighted POI** features. Here the POI feature is assigned weights based on importance score (%) is calculated out of 18 (sum of weightages)
Basis the score, defined as High, medium, low
- **High POI** - Area with more facility and higher population
- **Medium POI** - Area with average facility and average population
- **Low POI** - Area with low facility and low population

**OUTLET CLASSIFICATION:**
**Flagging outlets based on product type:**
- Outlets were flagged basis GSV contribution of product types (Impulsion/Restauration) they sell
- If majority GSV contribution (>70%) belongs to one product type, the outlet is flagged as that respective product type, else flagged as combined outlet

**Outlet Type Impulsion Products Restauration Products**
- Impulsion Outlet >70% <= 30%
- Restauration Outlet <=30% >70%
- Combined Outlet 30% - 70% 30% - 70% 
**Excluded Outlet Condition:**
- Outlets with <=0 GSV
- Outlets which started ordering after week 27 (June’21 end) were not considered in this classification

**Outlet classification based on performance (GSV)**
- Outlets are classified within each POI & Channel cross-section
- High (Chargers), Medium (Sprinter), Low (Stroller) and Very Low (Crawler) performance classification of outlet done based on condition table

- Charger - Top 60% contributors to GSV
- Sprinter - Next 20% Contributors to GSV
- Stroller - Next 15% Contributors to GSV
- Crawler - Bottom 5% Contributors to GSV
