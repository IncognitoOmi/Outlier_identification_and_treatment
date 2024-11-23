# Outlier Detection and Treatment

This repository focuses on detecting and treating outliers in a dataset using statistical techniques. It includes:

1. **Outlier Detection Methods**:
   - Z-Score Method
   - Interquartile Range (IQR) Method

2. **Outlier Treatment Approaches**:
   - Log transformation
   - Replacing Outliers (with median or other central tendencies)
   - Winsorization (Capping extreme values)

---

## **Outlier Detection Techniques**

### **Z-Score Method**
- Identifies outliers based on how far a data point deviates from the mean in terms of standard deviations.
- Threshold: Any value with a Z-Score > 3 or < -3 is considered an outlier.

### **IQR Method**
- Outliers are detected based on the interquartile range (IQR).
- Formula:
  - Lower Bound = Q1 - 1.5 * IQR
  - Upper Bound = Q3 + 1.5 * IQR
- Data points outside these bounds are treated as outliers.

---

## **Outlier Treatment Techniques**

### **1. Applying Log Transformation**
- Outliers are completely removed from the dataset.
- Useful when outliers are noise or errors.

### **2. Replace Outliers**
- Replace outliers with central tendency measures (e.g., median).
- Retains data size while reducing the impact of extreme values.

### **3. Winsorization**
- Caps outliers to the nearest boundary (upper or lower limit).
- Helps in reducing the effect of extreme values without removing them.

---

## **Key Benefits**
- Enhances model performance by handling noisy data.
- Improves the reliability of statistical summaries (mean, standard deviation, etc.).
- Provides a structured framework for data preprocessing.
