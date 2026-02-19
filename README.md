# Island Adventures 📍

This repository contains a **Jupyter Notebook (`island.ipynb`)** that simulates and analyzes **movement data** for a set of individuals — including visiting patterns to places like *Little Saint James Island* — using **fake sample data for fun and exploration**.

> ⚠️ **Disclaimer:** All data in this project is entirely *synthetic and fictional*. This notebook is intended for entertainment and learning purposes only. It does **not contain real personal data.**

---

## What This Does

The notebook:

* Generates **fake mobility data** for a group of people across a 14-day time window.
* Randomly assigns locations throughout the day and night.
* Defines **geofences** (e.g., Little Saint James Island, Zorro Ranch, Manhattan) using coordinates.
* Checks who has visited which areas.
* Identifies visits across multiple locations and outputs summary tables.

By the end you can see:
✔ Who “visited” the island
✔ When and for how long people were in specific zones
✔ A sample method to analyze geolocation datasets

---

## Core Features

### Synthetic Data Generation

Using Python, the notebook builds fake timestamps and GPS points across:

* Home locations (e.g., Miami, Denver)
* Work or travel places (e.g., NYC, Dallas)
* A geofence around Little Saint James Island

Example of setting up geofences:

```python
from shapely.geometry import Point, Polygon

island_poly = Polygon([
  (-64.830515, 18.304551),
  (-64.820305, 18.304482),
  (-64.819889, 18.296081),
  (-64.829742, 18.296586),
])
```

---

## What You’ll See

The workbook includes:

✔ A dataset of millions of “events”
✔ A geofence lookup to label visits (`is_island`, `is_ranch`, `is_nyc`)
✔ Filtering to find users who visited all three geofences
✔ Functions to compute likely sleep and work location patterns

---

## How to Run It

1. **Clone the Repository**

   ```bash
   git clone https://github.com/dmorton714/islandAdventures.git
   cd islandAdventures
   ```

2. **Open the Notebook**
   Start Jupyter and open `island.ipynb`:

   ```bash
   jupyter notebook
   ```

   or use GitHub’s built-in NB preview.

3. **Install Required Python Libraries**
   If needed:

   ```bash
   pip install pandas numpy shapely
   ```

---

## Why This Is Interesting

This project shows a fun way to:

* Simulate mobility timelines
* Cook up **fake location traces**
* Work with geospatial analysis without needing real sensor data
* Build foundational skills for location analytics workflows

Perfect for learning and exploring how real-world geolocation analytics might work!

---

## Notes

* The locations and paths are **completely simulated**.
* No personal data is stored or processed here — everything is placeholder/demo data.

---

If you want, I can also generate a **Badges section**, a **project logo**, or help you add a **project description for GitHub SEO**! 🏝️🚀
