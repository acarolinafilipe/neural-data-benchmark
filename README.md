# Large Scale Neural Data Benchmark

Data Engineering and Benchmark models for neural data analysis


## Data Engineering


**Datasets** 

| Study | Regions | Tasks | # Individuals | # Sessions | # Units |  # Spikes| # Behavior| Timepoints|
| :---:         |     :---:      |          :---: |  :---: |:---: |:---: |:---: |:---: |:---: |
[Perich et al.](https://dandiarchive.org/dandiset/000688)|	M1, PMd	| Center-Out, Random Target |	4	| 117	| 11,557|	143M|	20M|
[Churchland et al.](https://dandiarchive.org/dandiset/000070)|	M1	|Center-Out|	2|	9	|1,728|	706M	|87M|
[Makin et al.](https://zenodo.org/records/583331)	| M1, S1 |	Random Target| 	2	| 47	|14,899|	123M|	15M|
[Flint et al.](https://crcns.org/data-sets/movements/dream/welcome-to-dream)|	M1	| Center-Out|	1	|5	|957|	7.9M	|0.3M|
[NLB-Maze](https://neurallatents.github.io/datasets.html#mcmaze)|	M1|	Maze|	1|	1|	182	|3.6M|	6.8M|
[NLB-RTT](https://neurallatents.github.io/datasets.html#mcrtt)|	M1, S1|	Random | Target	|1|	1	|130|	1.5M	|2.8M|
[Ma Xuan et.al](https://datadryad.org/stash/dataset/doi:10.5061/dryad.cvdncjt7n) | M1 |  isometric wrist,grasping ,center-out,random-target | 6 | 96 | | | | |
[Chowdhury et al.](https://datadryad.org/stash/dataset/doi:10.5061/dryad.nk98sf7q7) | S1| reaching | 2|
[Gallego-Carracedo et al.](https://datadryad.org/stash/dataset/doi:10.5061/dryad.xd2547dkt)|M1, S1, PMd | reaching | 4 |






**Data Integration**
- combine data from multiple sources (files, databases, etc.) 
- create mappings between different data structures (schema matching)

**ETL**
- Extract, Transform and Load (ETL) process to a mediated schema for standardize data.

> [!NOTE]
> The standardized data can be found in the folder **Data**.

**API**
Automate preprocessing steps through a custom API with default functions.




## Benchmarks
Benchmark models for population and individual neurons

**LNP** 
Poisson Generalized Linear Model (aka Linear Non-Linear Poisson). 
![image](https://github.com/acarolinafilipe/neural-data-benchmark/assets/67625079/2a36e463-ee56-4dad-a51d-de9992d9b987)

**GLM** 
Autoregressive Poisson Generalized Linear Model.

![image](https://github.com/acarolinafilipe/neural-data-benchmark/assets/67625079/2d1862f3-2c16-45c0-b6e7-19a205932f20)

- Basis Functions: Raised Cosines,
- Non-Parametric GLM

**multi-filter LNP**

• responses may depend on more than one projection of stimulus! 
• emphasis on dimensionality reduction

![image](https://github.com/acarolinafilipe/neural-data-benchmark/assets/67625079/ff620abf-6479-4b46-8251-50a49630a026)

- Generalized Quadratic Model (GQM)
- Spike-triggered covariance (STC)

**Multi-Neuron GM**
Autoregressive Poisson Generalized Linear Model with coupling filters.

![image](https://github.com/acarolinafilipe/neural-data-benchmark/assets/67625079/d7b050e6-16d5-481a-8433-c2080a05b987)

- Low-rank

**deep learning / deep neural networks (DNNs)**

- CNN

![image](https://github.com/acarolinafilipe/neural-data-benchmark/assets/67625079/729700b5-2664-40a0-a680-99c40488d63d)

**Link Functions**

- exponential
- elliptical

**Metrics** 
Log-likelihood (bits/spikes), forecast power in 5 horizons (1, 5, 10, 100, 200 time steps), %Variance Explained, Pearson Correlation Coefficient, ROC Curve

