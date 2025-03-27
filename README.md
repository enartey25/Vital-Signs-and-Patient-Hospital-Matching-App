Vital Signs and Patient-Hospital Mapping Application

In Ghana, hospital beds are sometimes filled to the brim, especially in the emergency ward of public hospitals. This means that patients who are brought in from far in ambulances are sometimes turned away since they cannot be accommodated, which sometimes leads to the unfortunate death of patients. 

There should thus be a way for prospective patients and paramedics to be routed to hospitals based on proximity and availability of resources.

This project, however simple it may seem, aims to address the gap in communication between prospective patients, paramedics, and hospital staff concerning the availability of facilities.


Installation Instructions and Usage

To compile and run the application, the following libraries must be installed properly:

Kivy - The framework for the development of the application.
Webbrowser - Opens URLs in a web browser.
Time - Allows for time-related functions.
Math - Provides math functions and constants.
OS - Interacts with the operating system for file management.
Python-docx - Creates and edits Microsoft Word documents.
Selenium - Used to interact with web elements using XPath.
Geopy - Extracts the coordinates of the user.


Health Facilities Regulatory Agency (HeFRA) hospitals have been put in a 2D list with their respective Google Form links, latitudes, and longitudes to help in easy computation of locations.

The application first asks the user to input their credentials and vitals, namely,  name, blood pressure, temperature, pulse rate, oxygen saturation and a summary of how the patient is doing/feeling, The application then asks the user for their location, and routes them to the nearest hospital based on their location and the resources available. 

The patient’s data is sent to the appropriate hospital via a Google Form for their perusal, and is saved locally temporarily for future use. 

In case the patient’s vitals are needed, the user can simply enter the name of the patient to access their data in a Word document format.

Python was selected as the programming language since it is easy to write and maintain. It also allows for a prototype to be developed before making the final product.

The app was developed using Kivy, a Python framework that is used for the development of Android and iOS applications due to its widget-based design.


Contributing Guidelines and Reecommendations

I was unable to get the Google Maps API to work. Hence,  I worked around it and used Geopy and the Haversine distance formula to calculate the distance between the patient and each hospital and select the smallest distance. The disadvantage is that it only accounts for the straight line distance between points and not the various turns the patient might take. This could mean the closest hospital would be miscalculated if the user is between two relatively close hospitals. Geopy also picks a specific location within the town specified, and not the actual location of the user. I recommend that anybody who works further on this project uses the Google Maps API to rectify this error.

So far, all test cases have been run locally on a laptop, and not on a mobile device. Therefore, I recommend that the application be tested on a mobile device.

Data from HeFRA could be converted into the CSV format. The Pandas Library could then be used to sort out this data, thus eliminating the need for a list.

A decentralized database system could be integrated into the application to store the patient data, instead of using Google Forms to send the data to the respective hospitals. The patient would reserve the right to grant access to any health facility that would like to access their records.

A system linked to the hospital’s management records could be introduced to provide real-time updates to availability of beds.




Licensing

Permission is hereby granted, free of charge, to any person accessing this repository and associated documentation files, to use and modify copies of the repository. 







 




