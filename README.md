
#  UIDAI 2026: Aadhaar Inclusion Command Centre

**A Triangulated Geospatial Priority Model for Universal Enrollment**

##  Executive Summary

As Aadhaar reaches peak saturation, the "Final Mile" of inclusion becomes the most challenging. This project provides a **Strategic Risk Framework** to identify districts where 2026 population growth will outpace current enrollment infrastructure. By triangulating **biometric failure rates**, **demographic shifts**, and **geospatial accessibility**, we provide UIDAI with an actionable "Command Centre" to deploy resources efficiently.

##  Key Features

* **Triangulated Risk Scoring:** A multi-factor algorithm calculating inclusion risk  based on projected enrollment gaps and biometric friction.
* **National Heatmap:** Interactive choropleth map identifying "Red Zones" requiring immediate intervention.
* **Policy-Driven Action Plans:** Automated generation of district-specific strategies (e.g., *Mobile Van Deployment* vs. *Hardware Refresh*).
* **Executive Dashboard:** A Gradio-powered UI for regional directors to filter and analyze priority zones in real-time.

##  Technology Stack

* **Data Processing:** `Pandas`, `NumPy`
* **Geospatial Analysis:** `Folium`, `GeoPandas`, `JSON/GeoJSON`
* **Visualization:** `Plotly`, `Matplotlib`
* **Interface:** `Gradio` (for the Command Centre UI)

##  Project Structure

```text
├── data/
│   ├── Full_Aadhaar_Inclusion_Action_Plan.csv  # Final output with risk scores
│   └── india_states.geojson                     # Geospatial boundaries
├── notebooks/
│   └── Aadhaar_Analysis_Final.ipynb             # Full analysis & mapping code
├── README.md                                    # Project documentation
└── app.py                                       # Gradio Dashboard script

```

##  Methodology

Our model uses a normalized index  to rank districts:

1. **Demographic Load:** Projected 2026 population vs. current active Aadhaar IDs.
2. **Biometric Friction:** Historical failure rates in Fingerprint/IRIS authentication (signaling hardware aging).
3. **Inclusion Gap:** Identifying un-enrolled pockets in remote/tribal belts.

##  Strategic Recommendations

| Risk Level | Action Required | Resource Allocation |
| --- | --- | --- |
| **Critical (0.7 - 1.0)** | Mobile Enrollment Vans | High (Emergency Fund) |
| **Moderate (0.4 - 0.7)** | Sensor/Hardware Refresh | Medium (OpEx) |
| **Low (0.0 - 0.4)** | Baseline Maintenance | Standard (Routine) |

##  How to Run

1. Clone the repository:
```bash
git clone https://github.com/your-username/uidai-inclusion-2026.git

```


2. Install dependencies:
```bash
pip install pandas folium gradio requests

```


3. Run the Dashboard:
```bash
python app.py

```



---

