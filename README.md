# Urban-parking-dynamic-pricing
# 🚗 Dynamic Pricing for Urban Parking Lots

**Capstone Project – Summer Analytics 2025**  
Developed by **Sirshapan Kunda Roy** using Python, Pandas, NumPy, and Geopy.

---

## 📌 Overview

This project implements a real-time dynamic pricing engine for 14 urban parking lots based on occupancy, queue length, traffic, vehicle type, and competitor pricing. It helps reduce overcrowding and optimize utilization by updating prices dynamically every 30 minutes.

---

## 🛠 Tech Stack

| Layer            | Tools / Libraries                   |
|------------------|-------------------------------------|
| Programming      | Python 3.10                         |
| Data Handling    | pandas, numpy                       |
| Geolocation      | geopy                               |
| Visualization    | matplotlib                          |
| Platform         | Google Colab                        |
| Dataset Source   | Provided by Summer Analytics 2025   |

---

## 📐 Architecture Diagram

```mermaid
flowchart TD
    A[Raw CSV Dataset] -->|Ingested into| B[Google Colab]
    B --> C[Feature Extraction]
    C --> D[Model 1 - Baseline Linear Pricing]
    C --> E[Model 2 - Demand-Based Pricing]
    C --> F[Model 3 - Competitive Pricing]
    D --> G[Price Output]
    E --> G
    F --> G
    G --> H[Matplotlib Plot]
