# DecodeLabs — Data Analytics Project 1
## Data Cleaning & Preparation

---

## 📌 Project Overview

This is my **first project** as a Data Analytics Intern at **DecodeLabs**. The goal was to transform a raw, messy sales dataset into a production-ready "Gold Standard" dataset by mastering the art of data cleaning.

> *"80% Cleaning & Wrangling | 20% Analysis & Modeling"* — DecodeLabs

---

## 🎯 Project Objective

Clean a raw dataset by:
- ✅ Identifying missing/null values
- ✅ Removing duplicate records
- ✅ Correcting data formats (dates, numbers, text)
- ✅ Documenting every change (Change Log)

---

## 📊 Dataset Information

| Aspect | Details |
|--------|---------|
| **Source** | DecodeLabs Industrial Training Kit |
| **Format** | Excel (.xlsx) |
| **Initial Rows** | 1200 |
| **Initial Columns** | 14 |
| **Final Rows** | 1200 |
| **Final Columns** | 14 |

### Columns:
`OrderID`, `Date`, `CustomerID`, `Product`, `Quantity`, `UnitPrice`, `ShippingAddress`, `PaymentMethod`, `OrderStatus`, `TrackingNumber`, `ItemsInCart`, `CouponCode`, `ReferralSource`, `TotalPrice`

---

## 🔧 Tools Used

| Tool | Purpose |
|------|---------|
| **Google Colab** | Interactive notebook environment |
| **Python 3** | Programming language |
| **Pandas** | Data manipulation & cleaning |
| **NumPy** | Numerical operations |
| **ReportLab** | PDF generation (Change Log) |

---

## 📋 Cleaning Steps Performed

| Phase | Action | Impact |
|-------|--------|--------|
| **Phase 1** | Filled 309 missing values in `CouponCode` with 'No Coupon' | Preserved all records |
| **Phase 2** | Verified & removed duplicate `OrderID` records | 0 duplicates remaining |
| **Phase 3a** | Converted `Date` to datetime64[ns] (ISO 8601) | Enables time-series analysis |
| **Phase 3b** | Rounded `UnitPrice` & `TotalPrice` to 2 decimals | Consistent currency format |
| **Phase 3c** | Standardised text columns (strip + title case) | Prevents groupby/merge errors |

### Text columns standardised:
- Product
- PaymentMethod
- OrderStatus
- ReferralSource
- ShippingAddress

---

## ✅ Quality Gates (Zero Error Rate)

As required by DecodeLabs:

| Requirement | Status |
|-------------|--------|
| 0% error rate on Unique Identifiers | ✅ PASS |
| 0% error rate on Date Formats | ✅ PASS |
| Zero missing values | ✅ PASS |
| Zero duplicate OrderIDs | ✅ PASS |

---


