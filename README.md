# Zoology
from pathlib import Path

readme_en = """# Species Distribution Modeling — Occurrence Records

This repository contains an **R script** developed in the context of a **Graduate Course in Species Distribution Modeling**. The main goal of the code is to retrieve, filter, clean, and organize species occurrence records within a study area defined by a geographic polygon.

**Author:** X  
**Course:** Species Distribution Modeling  
**Level:** Graduate Program  

---

## Script objective

The script performs the following steps:

1. Loads a study-area polygon in shapefile format;
2. Retrieves species occurrence records from **GBIF**;
3. Filters records by time period;
4. Removes records without valid geographic coordinates;
5. Applies spatial cleaning procedures using the `CoordinateCleaner` package;
6. Retains only records located within the study-area polygon;
7. Generates a map with the final occurrence points;
8. Saves the filtered data in an `.xlsx` spreadsheet.

---

## Study area

In this version of the script, the study area is the **state of São Paulo, Brazil**, represented by the shapefile:

```text
SP_UF_2025.shp
