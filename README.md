# SOLARIS[Main Repo In Progress(will update it soon)]

### Exploring the Sun, Space Weather and Its Effects on Earth.

**SOLARIS** is a space-weather monitoring website that brings solar activity, space-weather events and scientific data together in one place.

🌐 **Live Website:** [Visit SOLARIS](YOUR_WEBSITE_URL)

---

## About the Project

I started building SOLARIS out of curiosity about the Sun and how its activity affects Earth.

Solar flares, coronal mass ejections, solar wind and geomagnetic storms are constantly changing. Understanding these events usually means looking through different scientific websites and datasets.

SOLARIS aims to bring that information into a single interactive website.

It combines data from NASA, NOAA and GFZ Potsdam with an interactive 3D solar system, charts, historical analytics and an experimental machine-learning feature.

This project is still under development, and I'll keep adding improvements as I work on it.

## Features

### 1. Space Weather Dashboard
- Overview of current space-weather conditions.
- Solar X-ray and proton flux monitoring.
- Solar wind speed, density and temperature.
- IMF Bz and geomagnetic activity.
- Kp index monitoring.
- Space-weather alerts.

### 2. Interactive 3D Solar System
- Explore the Sun and all eight planets.
- Planet rotation and orbital movement.
- Interactive camera controls.
- Clickable planets with information.
- Different viewing modes.
- Interactive solar-system visualisation.

### 3. Solar Activity Monitoring
- X-ray flux observations.
- Solar flare information.
- Active solar regions.
- Solar imagery from NASA SDO.

### 4. Space Weather Events
- NASA DONKI event information.
- Coronal Mass Ejection (CME) monitoring.
- Solar flare event records.
- Event details and timestamps.

### 5. Solar Wind and Geomagnetic Data
- Solar wind speed and density.
- Interplanetary magnetic field (IMF Bz).
- Geomagnetic activity.
- Dst and Kp index information.
- Aurora-related conditions.

### 6. Historical Analytics
- Historical space-weather measurements.
- Interactive charts.
- Changes in solar and geomagnetic conditions.
- Data-based exploration.

### 7. Experimental Kp Prediction
- Machine-learning-based Kp index prediction.
- Historical Kp data from GFZ Potsdam.
- Ridge regression model.
- Comparison against a persistence baseline.

*The prediction feature is experimental and is not an official space-weather forecasting service.*

---

## How SOLARIS Works

SOLARIS collects information from external scientific data sources, processes it through a Python backend and displays it through an interactive web interface.

```text
       EXTERNAL DATA SOURCES
   ┌─────────┬─────────┬─────────┐
   │  NASA   │  NOAA   │   GFZ   │
   └─────────┴─────────┴─────────┘
                 │
                 ▼
          PYTHON + FLASK
       Data collection & processing
                 │
                 ▼
          DATABASE / API
        Storage and data handling
                 │
                 ▼
          WEB INTERFACE
       HTML · CSS · JavaScript
                 │
        ┌────────┼─────────┐
        ▼        ▼         ▼
     Dashboard  3D View  Analytics
                          │
                          ▼
                     Predictions
```

The website uses external data sources rather than generating random measurements. When a source is unavailable, its data status should reflect that instead of presenting made-up live values.

## Technologies Used

| Area | Technologies |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| 3D Visualisation | Three.js |
| Charts | Chart.js |
| Backend | Python, Flask |
| Data Processing | NumPy, Pandas, SciPy |
| Machine Learning | Scikit-learn |
| Database | SQLite, SQLAlchemy |
| External Data | NASA, NOAA, GFZ |

## Data Sources

SOLARIS uses publicly available scientific data and imagery.

| Source | Used For |
|---|---|
| [NASA DONKI](https://ccmc.gsfc.nasa.gov/tools/DONKI/) | Solar events and CME information |
| [NOAA SWPC](https://www.swpc.noaa.gov/) | Space-weather observations and measurements |
| [NASA SDO](https://sdo.gsfc.nasa.gov/) | Solar imagery |
| [GFZ Potsdam](https://www.gfz-potsdam.de/en/) | Historical Kp index data |

## Screenshots

A look at the different parts of SOLARIS.

### Main Dashboard
![SOLARIS Dashboard](assets/screenshots/dashboard.png)

### Interactive Solar System
![3D Solar System](assets/screenshots/solar-system.png)

### Analytics
![SOLARIS Analytics](assets/screenshots/analytics.png)

### Kp Prediction
![Kp Prediction](assets/screenshots/predictions.png)

### Space Weather Events
![Space Weather Events](assets/screenshots/events.png)

---

## Project Structure

This is the structure of the public showcase repository. The actual website source code is maintained separately in a private repository.

```text
SOLARIS-Showcase/
│
├── README.md
│
├── assets/
│   ├── logo/
│   │   └── solaris-logo.png
│   │
│   ├── screenshots/
│   │   ├── dashboard.png
│   │   ├── solar-system.png
│   │   ├── analytics.png
│   │   ├── predictions.png
│   │   └── events.png
│   │
│   └── preview/
│       └── solaris-preview.png
│
├── docs/
│   ├── FEATURES.md
│   ├── TECHNOLOGIES.md
│   ├── DATA-SOURCES.md
│   └── HOW-IT-WORKS.md
│
├── updates/
│   └── CHANGELOG.md
│
└── LICENSE
```

## Development Timeline

| Period | Work |
|---|---|
| November 2026 | Initial SOLARIS development |
| November 2026 | Dashboard and 3D solar-system visualisation |
| November 2026 | NASA and NOAA data integration |
| November 2026 | Analytics and event monitoring |
| In progress | Prediction module and further improvements |

I'll update this section as new features are added.

## Future Plans

SOLARIS is not finished yet. There are several things I'd like to work on next.

### Data and Monitoring
- [ ] Add more reliable historical datasets.
- [ ] Improve data refresh and caching.
- [ ] Add more solar observation parameters.
- [ ] Improve CME tracking and event details.
- [ ] Add better geomagnetic storm monitoring.

### 3D Solar System
- [ ] Improve planetary textures and lighting.
- [ ] Add more detailed information about planets.
- [ ] Improve camera movement and navigation.
- [ ] Add more solar observation views.
- [ ] Improve the overall visual experience.

### Machine Learning
- [ ] Improve the Kp prediction model.
- [ ] Test additional machine-learning approaches.
- [ ] Compare predictions with real observed values.
- [ ] Improve model evaluation and reliability.
- [ ] Explore longer-term historical patterns.

### Website Improvements
- [ ] Improve mobile and tablet support.
- [ ] Make the dashboard easier to navigate.
- [ ] Add more interactive charts.
- [ ] Improve loading speed and performance.
- [ ] Improve error handling when external APIs are unavailable.

## Important Notes

- The 3D solar system is an educational visualisation. Planet sizes and distances are not shown to astronomical scale.
- The Kp prediction feature is experimental, not an official forecast.
- External data availability depends on the respective providers.
- SOLARIS is an independent project and is not affiliated with NASA, NOAA or GFZ Potsdam.

## Project Updates

Development updates and improvements will be documented in:

[`updates/CHANGELOG.md`](updates/CHANGELOG.md)

## Credits

Thanks to NASA, NOAA, GFZ Potsdam and the developers of the open-source libraries used in this project.

## About This Repository

This is the public showcase repository for SOLARIS.

It contains project information, screenshots, documentation and development updates. The actual application source code is kept in a separate private repository.

---

**SOLARIS — A closer look at the Sun and the space around us.** 