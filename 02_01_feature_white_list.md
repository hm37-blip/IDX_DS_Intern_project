# 📊 Feature Selection

## 🎯 Target Variable

| Feature | Description |
|---------|-------------|
| **close_price** | Target variable to predict |

---

## 🏠 Core Features

| Feature | Description |
|---------|-------------|
| **PropertyType** | Residential |
| **PropertySubType** | Single Family Residence |

---

## 📌 Baseline Features

These are the primary structural features used in the baseline model.

- **LivingArea**
- **LotSizeSquareFeet**
- **BedroomsTotal**
- **BathroomsTotalInteger**

---

## ➕ Additional Features

Additional variables considered to improve model performance.

| Category | Features |
|----------|----------|
| 🏗️ Property Information | `YearBuilt`, `PropertyCondition` |
| 📍 Location | `Latitude`, `Longitude`, `PostalCode` |
| 💰 Financial | `AssociationFee` |
| 🚗 Parking | `ParkingTotal` |
| 🏢 Building Structure | `StoriesTotal` |
| 🌡️ Amenities | `HeatingYN`, `CoolingYN` |
