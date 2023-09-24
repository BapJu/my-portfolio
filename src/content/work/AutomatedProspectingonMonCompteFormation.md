---
title: Automated Prospecting on MonCompteFormation
publishDate: 2019-12-01 00:00:00
img: /assets/Automated_Prospecting_on_MonCompteFormation.png
img_alt: Image of the site moncompteformation
description: |
  Design and develop an automation tool to assist in the prospecting of trainers on the French government's "MonCompteFormation" platform. The aim is to identify trainers with sub-optimal profiles for further coaching and rebranding.
tags:
  - Python
  - Scraping
  - API
---
## Overview

The French state funds a training service, [MonCompteFormation](https://www.moncompteformation.gouv.fr/), dedicated to individuals who have worked and wish to continue their training. Given the vast number of trainers on this platform, there's a significant opportunity for trainers to optimize their profiles to attract more students. This project assists a client who offers coaching and rebranding services to such trainers, making it easier to pinpoint potential prospects.

## Key Features

1. **Platform Scraping & API Connection**: Leveraging tools like `Burp Suite` and `Postman`, the software connects directly to the MonCompteFormation platform's API to extract relevant trainer data.

2. **Advanced Search Filters**:
    - **Training Mode**: On-site or remote.
    - **Location**: Uses the INSEE API to filter trainers based on postal codes.
    - **Training Theme**: Allows targeted prospecting based on the subject of the training.

3. **Profile Optimization Analysis**: The tool identifies trainers with unoptimized profiles, looking for:
    - Raw, unformatted descriptions devoid of HTML.
    - Absence of profile pictures.
    - Missing videos or multimedia content.

4. **Excel Integration**: Extracted and processed data on potential prospects is organized and stored in an Excel sheet using `pandas`, making outreach and follow-up streamlined and efficient.

## Benefits

- **Targeted Outreach**: Ensures that only trainers with a real need for optimization are reached out to, maximizing conversion rates for the client's services.
- **Efficiency**: Automated data extraction and analysis speeds up the prospecting process manifold compared to manual methods.
- **Organized Data Management**: Excel storage means structured data ready for CRM integration or direct outreach campaigns.