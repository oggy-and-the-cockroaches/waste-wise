# WasteWise: AI Waste Sorting & Municipal Collection Route Optimizer
**Skill Lab Project • Team 27**
* **Nidhi Shedole** (25211A05DB)
* **B. Sreehitha** (26215A0548)

---

## 🎯 Problem Statement (Slide 3 & 4)
Municipal solid waste management currently experiences failures across two interconnected fronts:
1. **Improper Waste Segregation (Sorting Dilemma)**: Recyclable plastics, glass, metals, and compostable wet waste get mixed at the consumer level. Once contaminated, recyclables end up occupying landfill space, generating toxic leachate and greenhouse methane.
2. **Inefficient Garbage Collection Routes (Collection Dilemma)**: Sanitation trucks follow blind, static schedules. Trucks expend significant diesel and time visiting half-empty bins, while overflowing bins in dense corridors remain unserviced.

---

## 🚀 The WasteWise Solution (Slide 2 & 5)
WasteWise links **AI-based source sorting** with **geographical IoT collection optimization**:
* **Citizen Flow (Steps 1–3)**: Instant computer vision photo classification to recognize material categories (plastic, paper, metal, organic, hazardous, glass), assign the proper municipal bin (Blue, Green, Yellow, Red), and provide actionable preparation tips.
* **Municipal Collection Flow (Steps 4–5)**: Live bin fill sensors connected to a PostGIS spatial heuristic engine (Traveling Salesperson Problem / 2-Opt) that computes dynamic routes, reducing travel mileage, diesel fuel consumption, and carbon emissions.

---

## 🛠️ Architecture & Tech Stack (Slide 8 & 9)
* **Client Interface**: Pure HTML5, Modern CSS3 & Vanilla JavaScript (ES6+). Zero bloated AI-template dependencies.
* **API Engine (Backend Target)**: FastAPI async microframework delivering sub-50ms inference routing.
* **Computer Vision Tier**: Multi-class deep convolutional network for waste recognition.
* **Spatial Optimization**: PostGIS & Vehicle Routing Problem (VRP) solver.

---

## 🌍 UN Sustainable Development Goals (Slide 10)
* **SDG 11 (Sustainable Cities & Communities)**: Cleaner neighborhoods, zero unserviced overflowing street bins.
* **SDG 12 (Responsible Consumption & Production)**: Maximizes recycled material purity and minimizes landfill diversion loss.
* **SDG 13 (Climate Action)**: Quantifiable cuts in diesel truck transit kilometers and $CO_2$ vehicular emissions.

---

## 💻 Running the Application
Simply double-click [`index.html`](./index.html) or open it directly in any modern browser (Google Chrome, Microsoft Edge, Firefox, Brave, Safari):

```bash
# On Windows PowerShell
start index.html
```

Or serve with any lightweight static file server:
```bash
# Optional (Python 3)
python -m http.server 8000
```
Then navigate to `http://localhost:8000/`.
