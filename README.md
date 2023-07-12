# Multi-hazard
Machine Learning-based Multi-Hazard Loss Estimation with Seismic and Tsunami Monitoring Networks 
 
This repository contains MATLAB code for implementing the Random Forest algorithm for regression tasks to estimate building asset loss caused by earthquakes and tsunamis. 
Prerequisites To run the code in this repository, you need:
• MATLAB (2021 or higher)
Installation
Clone this repository to your local machine (required_data.mat and multihazardloss_estimation.m)
Open MATLAB and navigate to the repository folder
Usage
Load the dataset (required_data.mat) into MATLAB 
Open the ‘multihazardloss_estimation.m’ file in MATLAB
Set the option:
response region (1 for Iwanuma, 2 for Onagawa, and 3 for joint (Iwanuma + Onagawa)), 
loss type (1 for earthquake only, 2 for tsunami loss only, 3 for multi-hazard loss),
PGV size (0 for none, 1 for small, 3 for median, 5 for large),
S-net size (0,5,10,20,40 sensors),
and waiting time fixed at 5 minutes.
Example:
response_region = 3; 
loss_type = 3; 
PGV_size = 5;
S_net_size = 40;
The above option would be estimating the multi-hazard loss at the joint locations of Iwanuma and Onagawa with a large portion of ground-motion sites and 40 offshore sensors.
Run the ‘multihazardloss_estimation.m’ file in MATLAB
The results, including mean squared error, R-squared value, and scatter plot for comparing model performance will be displayed in the MATLAB console
Contact For any inquiries or questions, please contact Yao Li and Katsuichiro Goda at yli3285@uwo.ca, kgoda2@uwo.ca.
