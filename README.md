# HPM Workflow
This is the workflow of Housing Projection Model (HPM), developed by Rajiv Myana and Su Jeong Jo for the Horry County Government. Since zoning ordinances can vary significantly across different local governments, this guide is to provide a general workflow. We recommend you to adapt this process to align with your local regulations. <br/>

**Please see the sample scripts for the Major Residential District (MRD2) [`MRD2.txt`](MRD2.txt), which allows multiple housing types, and for Single Family (SF7) [`SF7.txt`](SF7.txt), which allows only one housing type. <br/>**

## 1. Prepare GIS data and refined Zoning Ordinances. <br/>
  - GIS data <br/>
    - Vacant parcels with zoning codes and land use codes (Assessor's data) <br/>
      - Remove public / local government owned parcels. <br/>
      - Remove open space parcels. <br/>
      - Remove approved parcels for residential development. <br/>
    - Flood Zones <br/>
    - Wetlands <br/>
  - Refined Zoning Ordinances
    - Zoning Code, Uses, Minimum Required Area, Minimum Development Area, Maximum Density, Maximum Lot Coverage, and Future Land Use <br/>
## 2. Remove vacant parcels that fall into the flood zones and wetlands. <br/>
## 3. Set maximum density using Future Land Use Map. <br/>
## 4. Calculate potential housing units for each parcel. <br/>
  - Exclude commercial area for applicable zoning districts. <br/>
  - Define proportions of each housing type, including the proportion for site constraints area, by each zoning district. <br/>
  - Define Minimum Required Area for each housing type by each zoning district. <br/>
  - Set Maximum Lot Coverage and Maximum Density for each housing type by each zoning district. <br/>
    - If there is maximum density regulation for zoning district, compare the maximum density for FLUM and zoning district and choose whichever is smaller. <br/>

**Outcome: The number of housing units for each housing type by each zoning district. <br/>**
## 5. Apply subdivisions (lot size). <br/>
  - Set the proportion for site constraints area based on the parcel size. <br/>
  - Calculate Single Family housing units for Minor and Major Developments. <br/>

**Outcome: The number of housing units for entire vacant parcels. <br/>**
