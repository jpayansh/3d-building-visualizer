# 🌍 3D Interactive Map Visualizer

### *(MapLibre GL JS + Three.js + Threebox + Turf.js)*

A fully interactive **3D geospatial visualization** built using **pure HTML, CSS, and JavaScript**—no backend required.
This project combines **MapLibre**, **Three.js**, **Threebox**, and **Turf.js** to render realistic 3D buildings, interactive markers, animated curved routes, and dynamic distance calculations.

---

## ✨ Features

### 🗺️ **1. Interactive 3D Map**

* Built with **MapLibre GL JS** (open-source Mapbox alternative)
* Satellite view via MapTiler
* Smooth zoom, rotate, pitch, and flyTo animations

### 🏢 **2. Realistic 3D Building Models**

* GLB/GLTF models loaded with **Three.js**
* Accurate geo-anchoring with **Threebox**
* Multiple structures: main building + surrounding landmarks
* Real-world scale, rotation, and orientation

### 📍 **3. Smart Markers & Modes**

Three viewing modes:

| Mode             | Description                                      |
| ---------------- | ------------------------------------------------ |
| **HOMES**        | Focus on the main building with auto rotation    |
| **NEARBY**       | Shows hospitals, malls, complexes, etc.          |
| **CONNECTIVITY** | Displays distant cities + curved animated routes |

Markers include:

* Click events
* Fly animations
* Route highlighting
* Real-time distance & travel time

### 📐 **4. Distance & Time Calculation**

Powered by **Turf.js**:

* Accurate geodesic distance
* Auto travel-time estimation
* Updates live in bottom UI panel

### 🌀 **5. Curved Animated Connectivity Routes**

* Custom **Bézier-based curve generator**
* Added wave noise for *Google-Maps-style wiggly lines*
* Each route has its own GeoJSON source
* Animated `line-dasharray` for flowing effect

### 🧩 **6. Clean UI + Smooth Interactions**

* Dynamic marker visibility per mode
* Live place name, distance, time display
* Models always rendered above map (custom threebox layer)

---

## 🛠️ Tech Used

| Technology                  | Usage                            |
| --------------------------- | -------------------------------- |
| **MapLibre GL JS**          | Base map rendering               |
| **Three.js**                | 3D model rendering               |
| **Threebox**                | Geospatial Three.js integration  |
| **Turf.js**                 | Distance + geometry calculations |
| **HTML / CSS / JavaScript** | Entire frontend                  |
| **GLB / GLTF**              | Architectural models             |

---

## 📁 Project Structure

```
/assets
   /models
   /icons
   /css
   /js
index.html
README.md
```

---

## 🚀 Getting Started

### **1. Clone the repository**

```bash
git clone https://github.com/jpayansh/3d-building-visualizer.git
cd 3d-building-visualizer
```

### **2. Open the project**

Just open `index.html` in any browser.

⛔ *No backend, server, or build tools required.*

---


## 💡 How It Works (High-Level)

1. MapLibre initializes a WebGL map
2. Threebox injects Three.js into the map render loop
3. GLB models are loaded + placed using geocoordinates
4. Markers are added for home, nearby places, and cities
5. Clicking marker:

   * Map flies to location
   * Distance is calculated
   * Travel time computed
   * Curved route drawn & animated

---

## 📦 Deployment

Because it's plain HTML/CSS/JS, deploy anywhere:

* GitHub Pages
* Netlify
* Vercel
* Cloudflare Pages
* Any static hosting

Example (GitHub Pages):

1. Go to repo → Settings → Pages
2. Select `main` → `/root`
3. Save
4. Your site is live 🎉

---

## 🤝 Contributing

Pull requests are welcome!
For major changes, please open an issue first to discuss the idea.

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 👤 Author

**Payansh Jain**
GitHub: [https://github.com/jpayansh](https://github.com/jpayansh)

