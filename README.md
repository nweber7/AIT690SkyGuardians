# DAEN690SkyGuardians
## DAEN 690 Capstone Project: AIRSPACE ICE SUPER SATURATED REGIONS CHARACTERISTICS (ISSRC) AND PREDICTIONS DASHBOARD

### ABOUT THE PROJECT:

Problem Description: Aircraft induced clouds (also known as contrails) contribute 2% to Earth’s anthropogenic global warming. Contrails effect on global warming is due to its contribution to radiative forcing through its ability to trap outgoing radiation emitted by the Earth's surface, creating a warming effect. Unlike CO2 and other greenhouse gases that take approximately 20 years from the date it is emitted to affect the Earth's temperature; the effect of contrails is immediate. Ice supersaturated regions (ISSR) create atmospheric conditions conducive to the formation and spreading of contrails. Although techniques such as navigation avoidance would allow for a reduction in contrail generation, little is known about ISSRs, especially as it relates to locating and predicting when they form. Until there is a better understanding of ISSR size, depth, location, time of day, and seasonal trends, the problem will continue to persist for airline companies to effectively implement navigation avoidance techniques to lower their environmental impact. 

Project Goals: The following are the two main goals of the project.

1.	Create an interactive dashboard which visualizes past ice supersaturated conditions from the two selected weather stations which are Buffalo and Upton, NY. Visualizations represented in the interactive dashboard would include:
    - A table of days in which ISSCs occurred.
    - A map which showcases the daily drift of days that recorded ISSCs.
    - A histogram showing the daily drift in miles of the weather balloon.
    - A stacked bar chart of the occurrences of ISSCs by month and time window. AM represents Midnight and PM represents Noon launches of radiosondes.
    - A pressure altitude chart showing the daily floor and ceiling of the ISSRs. When hovering over the chart, the temperature and relative humidity to ice to pressure altitude chart will be shown. 
    - A comparison page, which compares both Buffalo and Upton.
2.	Through machine learning, answer the following questions:
    - Through time series modeling, forecast future days of ice supersaturated conditions for that region where the weather station is located. 
    - Through classification modeling, determine if one weather station’s variables such as instances that localized area experienced ISSC and the vertical depth of those regions could predict instances of ISSC at the other weather station. 

### BUILT WITH:

•	Python 

•	Tableau 

### DATA SOURCE:

National Oceanic and Atmospheric Administration Integrated Global Radiosonde Archive (IRGA) Sounding Data: https://www.ncei.noaa.gov/products/weather-balloon/integrated-global-radiosonde-archive

### GETTING STARTED:

#### Navigation: The main branch features the following folders:

- README
    - Overview of the project and GitHub repository.
 - Code Uploads
    - Working code and uploads from developers. 
- Dashboard
    - Data files used for Tableau and working Tableau files.
- Datasets
   - Datasets used for project. Buffalo and Upton were IGRA Sounding Datasets used and could not be uploaded to GitHub due to files being too large, however can be downloaded from the NOAA website. Instructions to downloading the dataset can be found in the “Data Download” section. 
- ISSRC Stations Code
  - Code used to narrow down our search for two weather stations that fit the criteria of being located in the Northeast region of North America, within a few hundred miles apart from one another, and still actively recording data in 2024. 
- MAINCODE
   - This is the finalized preprocessing and data visualization code that was used for the Tableau interactive dashboard. 
- Modeling
   - This was where the code for the modeling was located. 

#### Instructions: 

Data Download:

1.	Access the data by clicking the NOAA IRGA link from above and navigate to the Sounding Data section on that page.
![image](https://github.com/nweber7/DAEN690SkyGuardians/assets/99131499/e1528feb-79b4-4d58-a53b-b76f28e27c9d)
2.	Download the following zip files:
a.	Buffalo = USM00072528-data.txt
b.	Upton = USM00072501-data.txt
3.	Unzip files to be used for the MAINCODE

MAINCODE:

There are three files in the Main Code file. The following are the instructions to run the code:

1.	DATA PREP AND VIZ MAIN CODE
    - Download the ipynb file and make sure to have all libraries downloaded.
    - Run code
    - Users will be prompted to enter the file name and station’s city name.
2.	MODELING MAIN CODE 1
    - Download the ipynb file and make sure to have all libraries downloaded.
    - From Datasets file, make sure to download “Buffalo_issr2021.csv”
    - Run code
3.	MODELING MAIN CODE 2
    - Download the ipynb file and make sure to have all libraries downloaded.
    - From MAINCODE file, make sure to download and run “2010_2024_Data_Exporter.” 
        - Download and make sure all libraries are downloaded.
        - Run code
        - Users will be prompted to enter the file name and station’s city name.
        - Input Buffalo and Upton’s txt files
    - Input file paths for both Buffalo and Upton
    - Run code

### INTERACTIVE DASHBOARD:

The interactive dashboard can be found following this link:
https://public.tableau.com/app/profile/rebecca.conn7255/viz/ISSRDashboard/ISSRAnalysis

### ACKNOWLEDGMENTS: 

The research group for this project was Data Analytics and Engineering Students studying at George Mason University. The instructor for this course was Professor Brett Berlin. The sponsor of this project was Dr. Lance Sherry, the Director at the Center for Air Transportation Systems Research at George Mason University.  
