# 2025 EY Open Science AI & Data Challenge: Cooling Urban Heat Islands

## **Overview**  
This repository documents my participation in the **2025 EY Open Science AI & Data Challenge**, focusing on the development of AI-driven solutions to mitigate the **Urban Heat Island (UHI) effect**. Through advanced data analytics and machine learning techniques, this project aims to provide actionable insights for urban cooling strategies, enhancing climate resilience in cities.  

## **Challenge Statement**  
The UHI effect exacerbates rising urban temperatures, impacting energy consumption, public health, and environmental sustainability. This challenge seeks to leverage AI and data science to:  
- Identify and analyze heat island patterns using geospatial and environmental datasets.  
- Develop predictive models to assess the impact of urban infrastructure on temperature variations.  
- Propose data-driven mitigation strategies for urban planners and policymakers.  

## **Data Sources**
Weather Data: OpenWeatherMap API

Satellite Imagery: Landsat 8, Sentinel-2

## **Training Data Features**
Geospatial: Longitude, Latitude

Temporal: Datetime

Environmental: UHI Index, Land Surface Temperature (LST)

Urban Metrics: Building density, floor area ratio, vegetation indices

## **Methodology**
**1. Data Preprocessing**

Extract areas of interest (e.g., Manhattan, The Bronx) using osmnx.

Merge weather and training data based on location and timestamp.

Compute urban metrics: building count, area, height, and compactness within a 700m buffer around each training point.

**2. Satellite Features & Indices**

Extract **NDVI, NDBI, NDWI, emissivity** from Landsat 8 & Sentinel-2.

Derive **Land Surface Temperature (LST)** for UHI analysis.

**3. Machine Learning Modeling**

Train a **Random Forest Regression** model to predict the UHI Index.

## **Project Impact**
**Urban Planners:** Design heat-resilient cities.
**Governments:** Prioritize climate adaptation projects.
**Communities:** Raise awareness of urban heat impacts.
