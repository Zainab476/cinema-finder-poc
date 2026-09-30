# 🎬 Cinema Finder POC

An interactive web application for locating nearby cinemas and displaying movie venues on an interactive map. Built as a proof-of-concept using React, MapLibre GL, and modern mapping tiles.

---

## 🚀 Features

- **Interactive Map View**: Displays cinema locations with custom markers using MapLibre GL.
- **Fly-to-Cinema Navigation**: Smoothly pans and zooms the camera directly to selected cinemas on click.
- **Cinema Details Panel**: View information and showtimes for selected venues.
- **Responsive Layout**: Optimized for desktop and mobile viewing.

---

## 🛠️ Tech Stack

- **Frontend**: React.js / JavaScript (ES6+)
- **Map Library**: [MapLibre GL JS](https://maplibre.org/)
- **Styling**: CSS3 / Tailored UI Components
- **Environment**: CodeSandbox / Vite

---

## 🐛 Recent Bug Fixes

### **MapLibre "Fly to Cinema" Fix**
- **Issue**: Resolved an unhandled map instance / coordinate error occurring during `map.flyTo()` execution when a user clicked on a cinema card or marker.
- **Resolution**:
  - Validated location coordinate order (`[longitude, latitude]`) passed into MapLibre.
  - Ensured `flyTo` triggers strictly after the map instance is fully initialized and loaded.
  - Added optional chaining safeguards for missing cinema coordinate data.

---

## 💻 Getting Started Locally

### Prerequisites

Make sure you have Node.js (v16+) installed on your system.

### Installation

1. **Clone the repository**:
   ```bash
   git clone [https://github.com/Zainab476/cinema-finder-poc.git](https://github.com/Zainab476/cinema-finder-poc.git)
   cd cinema-finder-poc
