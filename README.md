# Comparison-of-Satellite-and-Sensor-PM2.5-Data
Overview
This repository contains the code and data for a study comparing satellite-derived PM2.5 data with ground-based sensor measurements in Mainz, Germany. The study explores the accuracy, reliability, and discrepancies between these two data sources for monitoring air quality, specifically focusing on fine particulate matter (PM2.5). The findings are intended to contribute to better understanding of air pollution and its public health implications.

Objective
The main goal of this study is to critically evaluate the differences between satellite data and sensor-based measurements of PM2.5 concentrations, assess the compliance with World Health Organization (WHO) guidelines, and provide insights into the use of both data sources for air quality monitoring. The study aims to:

Investigate spatial and temporal patterns of PM2.5 pollution in Mainz.
Analyze the performance of SDS011 sensors and compare them to satellite observations from the Atmospheric Composition Analysis Group at Washington University.
Evaluate whether the PM2.5 levels exceed WHO air quality standards.
Key Findings
Satellite data consistently reported higher PM2.5 levels compared to ground sensors, likely due to broader spatial coverage.
The sensor data typically showed lower values but still exceeded the WHO air quality limits in several instances.
Both data sources reveal significant discrepancies, which emphasize the importance of integrating satellite and ground-based measurements to obtain a more accurate picture of urban air quality.
Data
The dataset includes PM2.5 concentrations measured by both satellite and ground-based sensors across various locations in Mainz. The satellite data provides monthly averages from 2017 to 2022, and the sensor data includes real-time PM2.5 measurements from SDS011 sensors deployed in the city.

Data Files:
satellite_data.csv – Contains monthly average PM2.5 values from satellite observations.
sensor_data.csv – Contains PM2.5 values from ground-based SDS011 sensors.
comparison_results.csv – Results of the comparison between satellite and sensor data.
Methodology
Data Preprocessing: The data from both sources were cleaned, aligned geospatially using KDTree, and averaged to match temporal resolutions.
Statistical Analysis: A paired t-test was conducted to evaluate whether there were significant differences between satellite and sensor data.
Visualization: Graphs and maps were created to display the spatial distribution of PM2.5 levels and the discrepancies between the two datasets.
Usage
To replicate the study, follow the steps below:

Clone this repository:
bash
Kopiera
git clone https://github.com/yourusername/PM25-Comparison.git
Install the required libraries:
bash
Kopiera
pip install -r requirements.txt
Run the analysis by executing the script compare_pm25_data.py:
bash
Kopiera
python compare_pm25_data.py
Dependencies
This study uses the following Python libraries:

Pandas – For data manipulation and analysis.
NumPy – For numerical operations.
Matplotlib – For creating visualizations.
Scipy – For statistical analysis (paired t-test).
Geopandas – For geospatial data analysis.
License
This project is licensed under the MIT License – see the LICENSE file for details.

Future Directions
This study provides foundational insights, but further research could include:

Regular calibration of low-cost sensors to improve accuracy.
Hybrid models that integrate satellite and sensor data to improve PM2.5 estimation.
Exploring the local pollution sources and their effects on sensor measurements.
Acknowledgments
I would like to thank Johannes Gutenberg University Mainz for the opportunity to conduct this research, and the Sensor Community for providing access to ground-based sensor data.

Contact
For any questions or further inquiries, please contact [Sahar Gerandanesh] at [danesh_afc@hotmail.com].

