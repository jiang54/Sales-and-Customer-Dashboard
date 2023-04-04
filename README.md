# Sales and Customer -Dashboard (Done by Qlik Sense)


![image](https://user-images.githubusercontent.com/24377958/229706818-55a732f6-4f18-4ad7-917a-a024b687ee49.png)
![image](https://user-images.githubusercontent.com/24377958/229706910-db0a1d8d-ce11-421d-8c5e-08acfc0b23ed.png)
![image](https://user-images.githubusercontent.com/24377958/229706970-433c8317-b409-4a7f-adb7-2280d61cc56b.png)
![image](https://user-images.githubusercontent.com/24377958/229707176-d866e1f9-d4c6-4b33-a775-deb2c15b0d5b.png)
![image](https://user-images.githubusercontent.com/24377958/229707250-e2860959-0a43-46de-a16f-62c150ae8a22.png)
![image](https://user-images.githubusercontent.com/24377958/229707320-4a934c04-2621-429e-aeaf-190e789c6e80.png)

# Story Telling
![image](https://user-images.githubusercontent.com/24377958/229707728-03cdcec4-dbf0-4dc3-b6a0-776328db09b6.png)
![image](https://user-images.githubusercontent.com/24377958/229707762-c0e8c349-ce28-4f1b-9933-926a59b4216c.png)
![image](https://user-images.githubusercontent.com/24377958/229707787-8b09d4c2-901e-4f0c-bfad-000305459268.png)
![image](https://user-images.githubusercontent.com/24377958/229707808-30552806-24e7-4dae-9ca1-45393e9ee5da.png)
![image](https://user-images.githubusercontent.com/24377958/229707894-b66ef6d2-c2d8-40ce-a431-b31a419d4c97.png)


![image](https://user-images.githubusercontent.com/24377958/229714694-9a7bbbad-f067-44cf-8d7c-a1b8d2c66d31.png)

# Sales and Customer -Dashboard (Done by Qlik Sense)

![image](https://user-images.githubusercontent.com/24377958/229694560-27108937-3d08-43da-9209-5d6630105487.png)
# Vaccination Dashboard
![image](https://user-images.githubusercontent.com/24377958/229694738-8615adbf-7ed3-4b82-92b6-8c59b19a740b.png)

# Table of Contents

- [Problem Statement](https://github.com/jiang54/Sales-and-Customer-Dashboard#problem-statement)
- [Data Sourcing](https://github.com/jiang54/Sales-and-Customer-Dashboard#data-sourcing)
- [Data Preparation](https://github.com/jiang54/Sales-and-Customer-Dashboard#data-preparation)
- [Data Modeling](https://github.com/jiang54/Sales-and-Customer-Dashboard#data-modeling)
- [Data Analysis](https://github.com/jiang54/Sales-and-Customer-Dashboard#data-visualization)
- [Data Visualization](https://github.com/jiang54/Sales-and-Customer-Dashboard#Data-Visualization)
- [Insights](https://github.com/jiang54/Sales-and-Customer-Dashboard#insights)
- [Data Source](https://github.com/jiang54/Sales-and-Customer-Dashboard#data-source)


---
# Problem Statement

In order to maintain the sales between us and the customers, the company needs extensive dashboards to better understand the customers.

---

# Data Sourcing

Qlik Sense Sample Data

---

# Data Preparation

Data transformation was done in Excel and the dataset was loaded into Qlik Sense for Visualization.

Possible KPIs include(but not limited to):
- Overall Sales
- Overall Margin
- Sales of Regions

Data Understanding with 5 datasets:

- `Cities` which has `6 columns and 100 rows` of observation

The tabulation below shows the `Cities` table with its column names and their description:
| Column Name    | Description                                                                                                      |
| -------------- | -------------------------------- |
| City | City name |
| City Code | Unique code for each city |
| Region | Region of the city |
| Latitude | Latitude of the city |
| Longitude | Longitude of the city |
| Desc | Description of the city location |

- `Customers` which has `3 columns and 684 rows` of observation

The tabulation below shows the `Customers` table with its column names and their description:

| Column Name     | Description                          |
|-----------------|--------------------------------------|
| Customer        | Name of the customer                 |
| Customer Number | Unique identification number of customer |
| City Code       | Code for the city where the customer is located |

- `Item master` which has `5 columns and 827 rows` of observation

The tabulation below shows the `Item master` table with its column names and their description:
| Column Name      | Description                                |
|------------------|--------------------------------------------|
| Item Number      | Unique identifier for the product          |
| Product Group    | Broad category of the product              |
| Product Line     | Sub-category of the product group           |
| Product Sub Group| Sub-group of the product line               |
| Product Type     | Specific type of product within the sub-group |

- `Sales rep` which has `1 column and 64 rows` of observation(Delimiter = ";")

The tabulation below shows the `Sales rep` table with its column names and their description:
| Column Name      | Description                                |
|------------------|--------------------------------------------|
| Manager | Manager's name |
| Manager Number | Unique identifier for the manager|
| Path | Hierarchy path of the manager |
| Sales Rep Name | Name of the sales representative |
| Sales Rep Name1 | Additional name of the sales representative |
| Sales Rep Name2 | Additional name of the sales representative |
| Sales Rep Name3 | Additional name of the sales representative |
| Sales Rep ID | Unique identifier for the sales representative |


---

# Data Modeling

After the dataset was cleaned and transformed, it was ready to be modeled.
The fact and dimension have been combined into one table and is shown in the data model below
the connection part will be City code(cities to Customer), Item Number(Item master to Sales), Customer Number(Customer and Sales),Sales Rep ID(Sales and Sales Rep)

![image](https://user-images.githubusercontent.com/24377958/229714694-9a7bbbad-f067-44cf-8d7c-a1b8d2c66d31.png)



# Data Analysis
Add Necessary Measures


| Measure                    | Description                                                                                                                        |
| --------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
| Profit Margin                | (Sum(Sales)-Sum(Cost))/Sum(Sales) |


# Data Visualization
I show the KPIs, e.g. total sales, total margin, profit margin. Furthermore, I add the filter Pane to help better understanding, and horizontal combo chart, bar chart, map, pie chart, tree map, scatter plot, K-means to make it more readable.

![image](https://user-images.githubusercontent.com/24377958/229706818-55a732f6-4f18-4ad7-917a-a024b687ee49.png)
![image](https://user-images.githubusercontent.com/24377958/229706910-db0a1d8d-ce11-421d-8c5e-08acfc0b23ed.png)
![image](https://user-images.githubusercontent.com/24377958/229706970-433c8317-b409-4a7f-adb7-2280d61cc56b.png)
![image](https://user-images.githubusercontent.com/24377958/229707176-d866e1f9-d4c6-4b33-a775-deb2c15b0d5b.png)
![image](https://user-images.githubusercontent.com/24377958/229707250-e2860959-0a43-46de-a16f-62c150ae8a22.png)
![image](https://user-images.githubusercontent.com/24377958/229707320-4a934c04-2621-429e-aeaf-190e789c6e80.png)

Furthermore, I use the storying-telling to make a presentation.

![image](https://user-images.githubusercontent.com/24377958/229707728-03cdcec4-dbf0-4dc3-b6a0-776328db09b6.png)
![image](https://user-images.githubusercontent.com/24377958/229707762-c0e8c349-ce28-4f1b-9933-926a59b4216c.png)
![image](https://user-images.githubusercontent.com/24377958/229707787-8b09d4c2-901e-4f0c-bfad-000305459268.png)
![image](https://user-images.githubusercontent.com/24377958/229707808-30552806-24e7-4dae-9ca1-45393e9ee5da.png)
![image](https://user-images.githubusercontent.com/24377958/229707894-b66ef6d2-c2d8-40ce-a431-b31a419d4c97.png)
![image](https://user-images.githubusercontent.com/24377958/229714694-9a7bbbad-f067-44cf-8d7c-a1b8d2c66d31.png)


# Insights

- The number of transactions has been relatively flat from 2012 to 2014, with a profit margin of 41.28%.
- The United States accounts for 45.5% of our transactions, followed by the UK at 26.9% and Japan at 11.3%.
- The main products being sold are vegetables, fruit, canned shrimp, and meat - mainly everyday food items. If categorized broadly, the main categories are produce, canned products, deli, and frozen foods.
- The number of large customers is relatively small, with the vast majority being small customers.
# Data Source

Qlik Example Dataset
