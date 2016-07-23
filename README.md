# engine_analysis
Analysis of WRX engine data logs

## Setup:
1. create a fresh conda environment:<br>
  ```bash
  conda create -n engine python=3
  ```
2. snapshot the environment:<br>
  ```bash
  conda env export > environment.yml
  ```
3. or create the env from a snapshot:<br>
  ```bash
  conda env create -f environment.yml
  ```
