# GDSC-Scores-Analysis

### Dashboard Link : https://app.powerbi.com/view?r=eyJrIjoiZDI0MTc1ODQtNDJjYS00MDJhLTk3ZjQtNjY1ODY2MmE3YmI0IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9
## Problem Statement

This dashboard helps the airlines understand their customers better. It helps the airlines know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area. It also lets them know the average delay & departure time, thus since by using this dashboard they have identified this problem, they can further work on factors responsible for these unwanted delays.

Since, number of neutral/dissatisfied customers (almost 57 %) are more than satisfied customers (around 43 %), thus in all they must work on improving their services. 

Also since average delay in arrival & departure both is 15 minutes, thus they must try to reduce it.


### Steps followed 

Step 1: Connect MongoDB Atlas to Power BI
- Install MongoDB BI Connector: Download and install MongoDB BI Connector from MongoDB website.

- Configure MongoDB BI Connector: Create mongosqld.conf with Atlas connection details (uri, bindIp, port).

- Start MongoDB BI Connector: Run mongosqld --config mongosqld.conf to start BI Connector.

Step 2: Load Data into Power BI Desktop from MongoDB Atlas
- Open Power BI Desktop: Launch Power BI Desktop.

- Get Data from MongoDB Connector: Select "Get Data", choose "MongoDB Database", enter 127.0.0.1:3307, and credentials.

- Select Database and Collection: Choose your Atlas database and collection, and load data into Power BI.

Step 3: Perform Data Profiling and Error Handling in Power BI
- Open Power Query Editor: Click "Transform Data" to open Power Query Editor.

- Enable Column Profiling: In View tab, enable "Column distribution", "Column quality", and "Column profile".

- Adjust Profiling Settings: Set "column profiling based on entire dataset" in Query Options > Data Load.

- Identify Errors and Empty Values: Review profiles; handle nulls for "Arrival Delay" as needed.

Step 4: Create Dashboard in Power BI
Navigate to Report View: Go to Report view after closing Power Query Editor.

- Apply Theme: Select a theme in View tab.

- Add Visuals: Drag fields to canvas; use ellipsis (...) to choose visuals.

- Add Visual Filters (Slicers): Add slicers for "Class", "Customer Type", "Gate Location", and "Type of travel".

- Add Card Visuals for Average Delay: Include card visuals for average departure and arrival delay.

- Arrange and Customize Visuals: Arrange and format visuals to create desired dashboard layout.

- Save and Publish (Optional): Save .pbix file locally; optionally, publish to Power BI service.
           
# Snapshot of Dashboard (Power BI Service)
![image](https://github.com/KeerthikaGoli/GDSC-Scores-Analysis/assets/141056292/731359ed-906d-478f-a36d-a00fd6bf240d)
