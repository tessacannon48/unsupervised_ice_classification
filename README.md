## About The Project

<p align="center">
<img src="https://github.com/tessacannon48/unsupervised_ice_classification/blob/main/k_means_clustering.png" alt="Alt Text" width="575" height="450">

This repository aims to use unsupervised machine learning techniques to classify sea ice and leads in satellite imagery and altimetry data from the Arctic. More specifically, this repository contains two Jupyter notebooks which first collocate Sentinel-3 altimeter data with Sentinel-2 optical data and then apply K-Means and Gaussian Mixture Models to both data types to attempt binary classification of sea ice and leads. Leads are an important part of the polar climate system, and accurately detecting them is crucial for marine navigation and ecosystem stabilization efforts. 

In satellite imagery, leads can be identified through visual inspection or automated image analysis techniques that detect differences in pixel values. Satellite radar altimetry measures surface height variations by transmitting radar pulses and analyzing the returning signals. Sea ice and leads can be distinguished based on differences in their radar backscatter signatures and elevation profiles.

Data collocation is performed in data_collection.ipynb. Modeling is performed in unsupervised_ice_classification.ipynb. In the modeling notebook, there will be two main tasks: 

  1. Discrimination of sea ice and leads based on image classification using K-Means and Gaussian Mixture Modeling on Sentinel-2 optical data.
  2. Discrimination of sea ice and leads based on altimetry data classification using K=Means and Gaussian Mixture Modeling on Sentinel-3 altimetry data.

For more details and discussion on methods and results, please see the notebook unsupervised_ice_classification.ipynb. 

For prior work on using supervised machine learning techniques to classify sea ice and leads, please see my YouTube tutorial below.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/fLVKjpqdGwI/0.jpg)](https://www.youtube.com/watch?v=fLVKjpqdGwI)

## Repository Structure
```
root/
├── README.md         # This file
├── data_collocation.ipynb    # Jupyter notebook containing code to download and preprocess dataset
├── unsupervised_ice_classification.ipynb    # Jupyter notebook containing code and analysis
├── k_means_clustering.png   # Figure for visualization

```
## Getting Started

### Install Packages

The following packages need to be installed to run unsupervised_ice_classification.ipynb: 

######
    !pip install rasterio
######
    !pip install netCDF4

### Data Source

<p align="center">
<img src="https://dataspace.copernicus.eu/sites/default/files/styles/opengraph/public/media/images/2023-03/og_share.png?itok=zjtW85Fb" alt="Alt Text" width="600" height="300">

Data is downloaded from the Copernicus Data Space Ecosystem. The data_collocation.ipynb notebook will download the image and altimeter satellite data needed for modeling. A username and password from an account registered with the Copernicus Data Space Ecosystem is required to run the data collocation notebook: https://dataspace.copernicus.eu/. 

## Notes
This project was created for educational purposes as part of a University College London course on AI for Earth Observation taught by Dr. Michel Tsamados. Significant portions of the code were provided as part of the assignment and are not my original work.   

## Contact

Tessa Cannon - tessacannon48@gmail.com

For any questions or feedback, feel free to reach out or open an issue in the repository.


