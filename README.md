# WasteWise: Intelligent Waste Sorting & Municipal Route Optimizer

WasteWise is a smart municipal waste management platform that combines edge computer-vision for source-level waste classification with spatial heuristics for fuel-efficient garbage collection.

---

## 🎯 The Problem
Municipal solid waste management experiences critical bottlenecks across two interconnected fronts:
1. **Source Contamination (Sorting Dilemma)**: Recyclable plastics, glass, metals, and compostable wet waste get mixed at the consumer level. Once contaminated, recyclables end up occupying landfill space, generating toxic leachate and greenhouse methane.
2. **Blind Collection Logistics (Collection Dilemma)**: Sanitation trucks follow blind, static schedules. Trucks expend significant diesel and time visiting half-empty bins, while overflowing bins in dense corridors remain unserviced.

---

## 🚀 The WasteWise Platform
WasteWise links **AI-based source sorting** with **geographical IoT collection optimization**:
* **WasteWise Vision**: Instant computer vision photo classification to recognize material categories (plastic, paper, metal, organic, hazardous, glass), assign the proper municipal bin (Blue, Green, Yellow, Red), and provide actionable preparation tips.
* **WasteWise Dispatch**: Live bin fill sensors connected to a PostGIS spatial heuristic engine (Traveling Salesperson Problem / 2-Opt) that computes dynamic routes, reducing travel mileage, diesel fuel consumption, and carbon emissions.

---

## 🛠️ Architecture & Tech Stack
* **Client Interface**: Pure HTML5, Modern CSS3 & Vanilla JavaScript (ES6+). Zero bloated external dependencies.
* **API Engine**: FastAPI async microframework delivering sub-50ms inference routing.
* **Computer Vision Tier**: Multi-class deep convolutional network for waste recognition.
* **Spatial Optimization**: PostGIS & Vehicle Routing Problem (VRP) solver.

---

## 🌍 UN Sustainable Development Goals Alignment
* **SDG 11 (Sustainable Cities & Communities)**: Cleaner neighborhoods, zero unserviced overflowing street bins.
* **SDG 12 (Responsible Consumption & Production)**: Maximizes recycled material purity and minimizes landfill diversion loss.
* **SDG 13 (Climate Action)**: Quantifiable cuts in diesel truck transit kilometers and $CO_2$ vehicular emissions.

---

## 💻 Running the Application

### Option 1: Standalone Browser Launch
Simply double-click [`index.html`](./index.html) or open it directly in any modern web browser:
```bash
# On Windows PowerShell
start index.html
```

### Option 2: Local HTTPS Python Server (Port 8001)
```bash
python https_server.py
```
Then open `https://localhost:8001/` in your browser.
