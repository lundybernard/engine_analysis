# engine_analysis
Analysis of 2004 Subaru WRX engine data logs

All data logs collected using a [COBB Accessport v3](http://www.cobbtuning.com/products/accessport/subaru-accessport-v3-ap3-sub-002)

## Engine:
The engine in question is HEAVILY modified.
- 2.5L Hybrid
- VF-52 Turbo
- Processwest TMIC
- Cobb UP->Back exhaust

## Setup:
1. create a fresh conda environment:<br>
  ```conda create -n engine python=3```
2. snapshot the environment:<br>
  ```conda env export > environment.yml```
3. or create the env from a snapshot:<br>
  ```conda env create -f environment.yml```


## Log Files:
### naming:
Logfiles will be in the following format <vehicle_name>_log.yyyyMMddHHmm.csv

### content:
- Character encoding is iso-8859-1
- the raw data from the AP has various column header names
- the final column header starts with "AP Info:" and contains the metadata for the logs
- Different logs may contain different sets of columns.
