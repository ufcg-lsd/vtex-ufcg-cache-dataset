# vtex-ufcg-cache-dataset

VTEX Cache Dataset

The collected cache workload has 56,311,983 records. This corresponds to a random sample of 10% of all cached requests for products of multiple tenant catalogs during the timeframe between December 13, 2022, 21:00, and December 14, 2022, 07:00 (GMT-3).

The data is organized in a single .csv file of size 5.3 GB - to optimize the storage and transmission, we compacted using .tar.gz format, reducing its size to 3.1 GB. 

The header of .csv file is the following:

| tenant | product | ts | size |
|:------:|:-------:|:--:|------|

The fields include request timestamp, tenant identifier, product identifier, and response size, as described in Table 1. These records correspond to requests for data from 23,493,139 different products belonging to 4,894 different tenants. We anonymized the dataset to protect business-sensitive information, specifically the identifiers (tenant ID and product ID).


|       Column       |    Type   |                            Description                            |
|:------------------:|:---------:|:-----------------------------------------------------------------:|
|  Request Timestamp | Timestamp | The Unix timestamp of the request arrival time at the cache layer |
|  Tenant Identifier |   String  |                  The requested tenant identifier                  |
| Product Identifier |   String  |                  The requested product identifier                 |
|    Response Size   |  Integer  |             The size of the returned response in bytes            |
Table 1. Data dictionary 

## This data will soon be available in this repository in May 2024
