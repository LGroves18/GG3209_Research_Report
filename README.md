# GG3209 Research Report : Residential Suitability in Dumfries, Scotland

Student ID: 230012841

Course: GG3209 – Spatial Analysis with GIS

## Overview

This repository contains the code and analysis for an independent research project assessing which areas around Dumfries, Scotland, are most suitable for new residential development when accounting for projected future flood risk from the River Nith.

**Research Question:** Which areas around Dumfries are most suitable for new residential development when accounting for projected future flood risk from the River Nith?

## Method Summary

A GIS-based Multi-Criteria Evaluation (MCE) was conducted, combining:

- **Spatial preprocessing in QGIS:** study area definition (5km buffer around Dumfries), data clipping, rasterisation, distance surface generation, and standardisation of suitability criteria.
- **Weighting and overlay in Python:** visualisation and some statistics.

**Continuous suitability factors** (standardised 0–1, equal weighting):
- Distance to roads
- Distance to the River Nith
- Distance to existing houses (OS Local)

**Boolean constraints** (hard exclusions):
- Slope exceeding 10°
- SEPA future (climate-change-adjusted) medium-likelihood river flood extent
- Existing built-up areas (OS Open Built Up Areas)
