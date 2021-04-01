# AIS
A data analysis method to process AIS data and capture traffic features.

Automatic Identification System (AIS) is a maritime safety and vessel navigation system that automatically sends an AIS record every 2 to 30 seconds based on vessel speed. Every AIS message includes static information, like MMSI, vessel name, vessel type, vessel dimensions, and dynamic information, namely date and time, longitude and latitude, speed, heading, and destination. The AIS data is available on the MarineCadastre.gov .

an AIS record can be denoted as c_i=(lng_i,lat_i,ν_i,datetime_i,MMSI_i,type_i ), where (lng_i,lat_i) are the longitude and latitude coordination of the ith  record, ν_i is its speed over ground (SoG),  datetime_i is the time and date of the record, MMSI_i is a unique ID number for the vessel corresponding to the ith record, and type_i is the vessel type (e.g. tanker, or cargo). 

![Picture1](https://user-images.githubusercontent.com/33292172/113235057-0e5a8700-9268-11eb-876d-0750a8309b67.png)

In this project, a fast algorithm is presented to analyze AIS data and separate them into tours and trips. The proposed algorithm also finds vessels directions as inbound, outbound, and stop. Using segmentation technique, we could analyze traffic behavior for the whole channel or specific segments to provide comprehensive or meticulous results. Finally, the methodology is applied to the Houston Ship Channel (HSC) as a case study with one month of AIS data, and traffic features such as travel speed, traffic density, traffic flow, trip attraction, trip generation, and Origin-Destination (O-D) matrices are quantified for different types of vessels with different widths and drafts at different segments.

<img width="1279" alt="Screen Shot 2021-03-31 at 9 36 24 PM" src="https://user-images.githubusercontent.com/33292172/113235685-2e3e7a80-9269-11eb-91e9-d7c1055e8e8b.png">


The simplified version of our algorithm is presented in the following flowchart.

![Picture2](https://user-images.githubusercontent.com/33292172/113235859-6f368f00-9269-11eb-8b0b-8e3732897ce6.png)
