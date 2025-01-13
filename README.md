# **Plasma Charge Neutralization Analysis**

This repository contains a Jupyter Notebook for analyzing the effectiveness of plasma treatments in neutralizing charges on various materials (e.g., insects and synthetic objects). This work is part of ongoing research in the niche field of bee electroreception.

## **Project Overview**

### **Background**
Bee electroreception is a highly specialized field with limited established methods. This study evaluates two methods for neutralizing charges to bring them as close to zero as possible:
1. **USB Plasma Method**: Using a plasma source (lighter).
2. **No Plasma Method**: Serving as a control, without using the plasma source.

### **Experimental Setup**
- **Materials**: Small and large bumblebees and nylon balls.
- **Equipment**:
  - **Faraday Pail**: Primary and most reliable charge measurement method.
  - **Ring Charge Sensor (RCS)**: Complementary but less accurate.
- **Procedure**:
  - Objects were charged using an ion gun.
  - Plasma treatment involved exposing objects to a USB lighter for 30 seconds, followed by charge measurements before and after treatment.

---

## **Data Description**

The dataset used in this analysis (`USB_plasma_data.csv`) contains the following columns:
- **`method`**: Indicates treatment type (`usb plasma` or `no plasma`).
- **`material`**: The type of object tested (e.g., bumblebee, nylon ball).
- **`size`**: The size of the object (`small` or `big`).
- **`faraday_charge_pC_before` / `faraday_charge_pC_after`**: Faraday Pail charge measurements before and after treatment (in picoCoulombs).
- **`calibratedcharge_before` / `calibratedcharge_after`**: Complementary RCS measurements before and after treatment (in picoCoulombs).

---

## **Repository Contents**

1. **`usb_plasma_analysis.ipynb`**: Jupyter Notebook containing:
   - Data exploration
   - Statistical analyses
   - Visualizations (boxplots, scatterplots)
   - Summary statistics 
2. **`USB_plasma_data.csv`**: The dataset
4. **`README.md`**: This documentation file.

---

## **Usage Instructions**

### **Prerequisites**
- Ensure Python 3.x and the following libraries are installed:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`
