
## 1. Target Variable
* **ClosePrice**: The amount of money paid by the purchaser to the seller for the property under the agreement. 

## 2. Key Baseline Features (Week 2 EDA Focus)
These fields are explicitly required by the project manual for initial data exploration. 
* **LivingArea**: The total livable area within the structure. 
* **BedroomsTotal**: The total number of bedrooms in the dwelling. 
* **BathroomsTotalInteger**: The simple sum of the number of bathrooms (e.g., a property with two Full Bathrooms and one Half Bathroom will be 3). 
* *Related granular fields*: **BathroomsFull**, **BathroomsHalf**, **BathroomsThreeQuarter**. 
* **LotSizeArea** / **LotSizeSquareFeet** / **LotSizeAcres**: Measurements representing the total area of the lot. 

## 3. Mandatory Filtering Fields
These fields must be used to isolate the specific subset of data required for the model. 
* **PropertyType**: A list of types of properties. (Must filter for `Residential`.
* **PropertySubType**: A list of property sub-types. (Must filter for `Single Family Residence`).

## 4. High-Potential Features for Advanced Engineering (Week 6+)
These variables are excellent candidates for capturing non-linear relationships, geographic premiums, and property depreciation during model optimization. 
* **YearBuilt**: The year an occupancy permit was first granted for the house. Essential for engineering a numeric `Property Age` feature. 
* **Latitude** & **Longitude**: The geographic coordinates of a reference point on the property.  Crucial for spatial joining with California School District boundaries. 
* **PostalCode** & **City**: The postal code and city in the listing address. Useful for regional grouping and categorical target encoding.
* **ElementarySchoolDistrict** / **HighSchoolDistrict**: School district catchment areas. A strong proxy for neighborhood desirability and local property taxes.
* **AssociationFee**: A fee paid by the homeowner to the Home Owners Association. Can indicate the presence of premium community amenities.
* **ParkingTotal** / **GarageSpaces**: The total number of parking spaces or garage spaces included in the sale. 
* **PropertyCondition**: A list describing the condition of the property and any structures included in the sale. 
