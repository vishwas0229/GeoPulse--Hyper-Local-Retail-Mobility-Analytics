

\# Day 9 – Spatial Catchment Analysis Validation



\## Objective

Validate the 500-metre store catchment analysis using GPS location data and geographical distance calculations.



\## Dataset

\- GPS records: 100

\- Unique devices: 100

\- Retail stores: 5

\- Missing values in cleaned GPS dataset: 0



\## Methodology

The Haversine formula was used to calculate geographical distances between GPS coordinates and store locations.



A device was considered within a store catchment when its calculated distance from the store was less than or equal to 500 metres.



\## Results



| Store | Devices within 500m |

|---|---:|

| Store A | 1 |

| Store B | 0 |

| Store C | 1 |

| Store D | 1 |

| Store E | 1 |



\- Total GPS-store comparisons: 500

\- Total detected devices within catchments: 4

\- Stores with no detected devices: 1

\- Shared devices across store pairs: 0



\## Validation

The independently calculated catchment counts matched the existing CSV outputs.



The Haversine distance calculation and 500-metre threshold were validated successfully.



\## Observation

Store A, C, D and E each had one detected device within their catchment areas. Store B had no detected device.



The dataset contains one GPS record per unique device. Therefore, these results represent detected devices rather than repeat customer visits.



\## Conclusion

The spatial catchment analysis was successfully validated. The results provide an initial understanding of store-level geographical coverage and can support further retail location analysis.



