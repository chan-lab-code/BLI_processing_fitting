This Jupyter notebook code written in python allows users to process and fit biolayer interferometry (BLI) binding kinetics data. 
This code was developed by Benjamin Stordy and Zahra Sepahi in the Chan lab at the Unversity of Toronto. 
This project is licensed under the terms of GPLv3. 

To use this code, first run the BLI_processing script to clean and prepare BLI data for fitting. Then, run the BLI_fitting code to extract binding constants from the data. 
Output files (.pdf files containing plots of the data and fitted curves, .txt and .xlsx files containing the fitting results) will be saved into the same folder as the data.

Before running the BLI_processing code, BLI data must be prepared in a CSV file in the following format:
* Timeseries data is presented in columns, with one row per timepoint
* The first column contains the timepoints and is labelled "Time"
* Subsequent columns contain the binding data with column labels that indicate whether the data is a sample or a control. Sample columns are prefixed "NP " and control columns are prefixed "A ". These prefixes are followed by the analyte concentration in Molar units. For example, "NP 1.0E-6" would indicate sample data at a concentration of 1.0E-6 M.
* Background measurements of sample and control without analyte (i.e. "NP 0" and "A 0") must be included.
