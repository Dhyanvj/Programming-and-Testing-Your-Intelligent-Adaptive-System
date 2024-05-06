# Programming-and-Testing-Your-Intelligent-Adaptive-System
1. The problem domain was to create a virtual house, particularly the environment
management within that house and include adaptation and intelligence within this
domain. You should use Java, Python or Anylogic for this software (if you would like
to use any other application this will need to be approved by the module leader) and
deliver all the required code in one zip file. It should read in the training file supplied
and calculate the an indoor temperature and humidity value every 15 minutes. This
should be output to a .csv file with one row for each 15 minute period containing the
indoor temperature and indoor humidity value of your virtual home.
2. You have 2 options for changing the temperature and humidity that operate under
the following assumptions:
a. Mechanical ventilation. This takes 15 minutes and causes the temperature
(and also humidity) to be equal to that of the outside. When this is turned off the
temperature and humidity return to the original values in 15 minutes.
b, Storage heaters. These take 15 minutes to increase the temperature by 0.5
degrees. This effect lasts 4 hours and can only be used twice per day.
Note, if both methods are used at once, the mechanical ventilation process takes
priority and negates the heating effects for remainder of the 4 hour period
The use of these options should be decided by the software.
Marks will be awarded for:
Presence of intelligent and adaptive behaviour (10 marks)
Improving the satisfaction of the user. This will be calculated using a hidden
formula based on the indoor temperature and humidity output from your software
(10 marks)
The usability and effectiveness of the code (10 marks)
Part 2. Short Report (10/40)
Deliver a short (less than 2 pages of A4) report on the performance of your solution.
What were the quantitative benefits of the approach and how well did it fit thr
qualitative requirements outlined in Assignment 1
-------
This project should be delivered as a zip file to canvas assignment 2. This zip file
should include:
All required software and a readme to enable the user to run it.
A short 2 page report detailing how your software meets the requirements of the
client, this should be as a pdf file.
A .csv file containing the indoor temperature, CO2 levels and humidity for your
virtual house for every 15 minute period from 13/03/2012 11:45 to 11/04/2012
06:30
The associated files include:
6com2007.csv gives a sample of some of the data available for the modelling process
Housemap.png gives a layout of the house
