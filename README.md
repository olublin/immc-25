# immc-25

This repository contains code for the problem 2 of the 2025 IMMC (Intercollegiate Mathematical Modeling Competition). The challenge for this problem was to develop a mathematical model or framework that uses publicly available data to identify Communities of Interest in North Carolina. 

Contributors: [Oliver Lublin](https://github.com/olublin), [Alex Zhang](https://github.com/Alexz08), and [Suhaib Mansour](https://github.com/Swabwayy). 


![alttext](https://t4.ftcdn.net/jpg/09/80/35/79/360_F_980357961_Fc0XgoAy4MAhEOarz4euTyzMob050W0x.jpg)

---
## Running graph_clustering.ipynb

This `graph_clustering.ipynb` script contains all necessary information to run the clustering algorithm on NC counties. As we have made use of the `pytidycensus` package to import census and geographic data for counties, no additional data sources are needed. 

The user must provide a census API key to utilize the pytidycensus package. An API key can be accessed at [https://api.census.gov/data/key_signup.html]. 

### Requirements

The required python libraries to run the script are:

- Pandas
- Geopandas
- Numpy
- Matplotlib.pyplot
- pytidycensus
- networkx
- sklearn.cluster

### Outputs

The script outputs the following .png files for the described graphs and maps:

- full_graph.png: Contains undirected base graph with edges connecting all counties
- weights_example.png: Contains zoomed-in graph of Triangle area with weights
- clustered_counties.png: Contains map of NC counties clustered into 14 districts by our algorithm.

### Framework

The algorithm this script utilizes to form clusters is based on modeling the map of counties using graph theory and cosine similarities and performing spectral clustering on the graph. More information about the framework behind this clustering algorithm can be found in the .pdf writeup. 


