# **Plasma Charge Neutralization Analysis**

This repository contains a Jupyter Notebook for analyzing the effectiveness of plasma treatments in neutralizing charges on various materials (e.g., insects and synthetic objects). This work is part of ongoing research in the niche field of bee electroreception.

## **Project Overview**

### **Background**
Bee electroreception is a highly specialized field with limited established methods. This study evaluates two methods for neutralizing charges to bring them as close to zero as possible:
1. **USB Plasma Method**: Using a plasma source (usb lighter).
2. **No Plasma Method**: Serving as a control, without using the plasma source.
   
### **Study Objectives**

#### 1. **Effectiveness of Charge Neutralization** - First cell of the IPython notebook executed in the JupyterLab environment
- **Question:** How close to zero are the charges after treatment?  
- **Purpose:** Evaluate the ability of plasma treatment to achieve charge neutrality, regardless of initial charge values.  
- **Logic:** Closer-to-zero charges after treatment indicate better neutralization.  
- **Outcome:**  
  - No significant differences were found between treatment groups (USB Plasma vs. No Plasma).  
  - Material type and size did not significantly affect charge neutralization (see code notes for detailed results and explanations).  

#### 2. **Magnitude of Charge Change** -  Second cell of the IPython notebook executed in the JupyterLab environment
- **Question:** How much does the treatment change the charge?  
- **Purpose:** Measure the magnitude of charge adjustment, whether positive or negative.  
- **Logic:** Evaluate the extent to which plasma treatment alters charges compared to no plasma, focusing on the overall impact.  
- **Outcome:**  
  - Plasma treatment has a significantly larger impact on larger objects.  
  - The effect on smaller objects was less pronounced and not statistically significant (see code notes for detailed results and explanations).  

### **Experimental Setup**
- **Materials**: Small and large bumblebees and nylon balls.
- **Equipment**:
  - **Faraday Pail**: Primary and most reliable charge measurement method.
  - **Ring Charge Sensor (RCS)**: Complementary but less accurate.
- **Procedure**:
  - Objects were charged using an ion gun.
  - Plasma treatment involved exposing objects to a USB lighter for 30 seconds, followed by charge measurements before and after exposure.

---

## **Data Description**

The dataset used in this analysis (`USB_plasma_data.csv`) contains the following columns:
- **`method`**: Indicates treatment type (`usb plasma` or `no plasma`).
- **`material`**: The type of object tested (`bumblebee` or `nylon ball`).
- **`size`**: The size of the object (`small` or `big`).
- **`faraday_charge_pC_before` / `faraday_charge_pC_after`**: Faraday Pail charge measurements before and after exposure (in picoCoulombs).
- **`calibratedcharge_before` / `calibratedcharge_after`**: Complementary RCS measurements before and after exposure (in picoCoulombs).

---

## **Repository Contents**

1. **`usb_plasma_analysis.ipynb`**: Jupyter Notebook containing:
   - Data exploration
   - Statistical analyses
   - Visualizations (boxplots, scatterplots)
   - Summary statistics 
2. **`USB_plasma_data.csv`**: The dataset
4. **`README.md`**: This documentation file.
5. **`LICENSE`**

---

## **Usage Instructions**

### **Prerequisites**
- Ensure Python 3.x and the following libraries are installed:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`
