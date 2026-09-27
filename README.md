# Watershed Impact Viewer

### Application of Geospatial Techniques for Visualization and Analysis of Geo-Coded Images to Enhance Watershed Development Outcomes

---

## Project Overview

Watershed development programs require reliable spatial information to understand changes in vegetation, water availability, land conditions, and the impact of watershed structures.

The **Watershed Impact Viewer** is a browser-based geospatial prototype designed to support visualization and analysis of watershed locations using geo-coded field images, satellite imagery, and before-and-after comparisons.

The prototype provides an interactive interface for:

- Selecting watershed/structure locations
- Uploading watershed data through CSV
- Processing geo-coded field photographs
- Visualizing before-and-after satellite imagery
- Analyzing vegetation/greenness changes
- Analyzing water-related changes
- Examining structure-level impact
- Comparing field/drone images
- Supporting spatial interpretation for watershed monitoring

---

# Problem Statement

### Application of Geospatial Techniques for visualization and analysis to interpret Geo-Coded Images to enhance watershed Development Outcomes

Watershed development in rural and semi-arid regions requires continuous monitoring of land use, drainage, vegetation, soil moisture, water bodies, and changes over time.

Traditional monitoring methods often depend heavily on:

- Field surveys
- Manual reporting
- Limited spatial coverage
- Time-consuming data collection
- Difficulty in comparing conditions over different periods

Geo-coded images combined with satellite-based spatial datasets can provide location-specific information that helps visualize and interpret watershed conditions.

The proposed approach aims to provide a systematic and scalable framework for integrating:

- GIS
- Remote sensing
- Geo-coded images
- Satellite imagery
- Thematic analysis
- Before-and-after comparison

to support improved watershed monitoring and assessment.

---

# Proposed Solution

The **Watershed Impact Viewer** provides an integrated browser-based interface for visualizing and analyzing watershed-related information.

The prototype allows users to provide watershed locations through a CSV file or manually enter coordinates. Geo-coded photographs can also be uploaded for extracting location information.

For a selected location, the system provides before-and-after visualization and analysis using satellite imagery and image-derived indicators.

### Key components

1. **Geospatial Location Input**
   - Upload watershed/state data using CSV.
   - Add locations manually using latitude and longitude.
   - Select locations interactively on the map.

2. **Geo-Coded Image Interpretation**
   - Upload field photographs containing GPS information.
   - Extract GPS coordinates from image metadata.
   - Provide OCR-based coordinate extraction when required.

3. **Satellite Visualization**
   - Display before-and-after satellite imagery for selected locations.
   - Support visual comparison of changes over time.

4. **Vegetation Analysis**
   - Analyze image-based vegetation/greenness indicators.
   - Display changes between the selected periods.

5. **Water Analysis**
   - Analyze water-related image indicators.
   - Visualize changes between before-and-after conditions.

6. **Structure-Level Analysis**
   - Examine the area around a selected watershed structure.
   - Compare the broader area with the immediate vicinity of the structure.

7. **Field and Drone Image Comparison**
   - Upload before-and-after field or drone images.
   - Compare image-derived vegetation and water-related indicators.

---

# Live Prototype

The working prototype can be accessed directly in the browser:

**[Open the Watershed Impact Viewer](https://satwiksinha097.github.io/watershed-impact-viewer/watershed-impact-viewer.html)**

The link opens the actual prototype interface hosted using GitHub Pages.

---

# Testing the Prototype

### Step 1 — Open the Prototype

Click the prototype link above

---

### Step 2 — Select Input Method

The prototype supports multiple ways to provide watershed information:

- Upload a watershed/state CSV file
- Add a location manually
- Select a location using the interactive map

---

### Step 3 — Test Geo-Coded Images

Upload a geo-coded field photograph.

The prototype can:

- Read GPS information from image metadata
- Identify geographic coordinates
- Use OCR-based coordinate extraction when GPS metadata is unavailable

---

### Step 4 — View Satellite Imagery

Select a location and the required before/after years.

The prototype provides satellite imagery panels for visual comparison.

---

### Step 5 — Analyze Vegetation

Use the vegetation analysis section to examine:

- Greenness
- Vegetation-related changes
- Before/after differences

---

### Step 6 — Analyze Water

Use the water analysis section to examine:

- Water-related indicators
- Before/after changes
- Spatial differences around the selected location

---

### Step 7 — Examine Structure-Level Impact

The prototype provides analysis at two spatial scales:

- Broader area around the selected structure
- Immediate vicinity around the structure

This helps visualize localized changes around watershed interventions.

---

### Step 8 — Test Field/Drone Images

Upload before-and-after field or drone images to compare:

- Vegetation/greenness
- Water-related indicators
- Overall image-derived changes

---

# Prototype Demonstration

A video demonstration of the prototype is available here:

**[Watch the Prototype Demonstration](https://drive.google.com/file/d/1EkKRAlKEEbOxW9gAsGzs5GR8EJ7P503W/view?usp=sharing)**

---

# System Workflow

```text
                ┌──────────────────────────┐
                │     User / Evaluator     │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │   Input Watershed Data   │
                │                          │
                │  • CSV                   │
                │  • Manual Location       │
                │  • Geo-Coded Image       │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │   Location Identification│
                │                          │
                │ • Latitude / Longitude   │
                │ • GPS Metadata           │
                │ • OCR Coordinates        │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │   Satellite Imagery      │
                │                          │
                │     Before / After       │
                └────────────┬─────────────┘
                             │
              ┌──────────────┼──────────────┐
              ▼              ▼              ▼
       ┌────────────┐ ┌────────────┐ ┌──────────────┐
       │ Vegetation │ │   Water    │ │  Structure   │
       │  Analysis  │ │  Analysis  │ │    Impact    │
       └──────┬─────┘ └──────┬─────┘ └──────┬───────┘
              │              │              │
              └──────────────┼──────────────┘
                             ▼
                ┌──────────────────────────┐
                │ Before / After Comparison│
                │                          │
                │   Visualization &        │
                │   Interpretation         │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │ Watershed Monitoring &   │
                │ Decision Support         │
                └──────────────────────────┘
