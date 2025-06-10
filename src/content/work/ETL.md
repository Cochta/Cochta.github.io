---
title: WhoFeedsMe
publishDate: 2012-10-02 00:00:00
img: /assets/ressources/ressourceETL/Logo.PNG
img_alt: Handmade logo
description: |
  I created an ETL (Extract, Transform & Load) as part of my studies in 2019
tags:
  - ETL
  - C#
  - SQL
  - MongoDB
---

### Overview

##### Initial Situation
As part of my **Federal VET Diploma (CFC)** in 2019, I was asked to create an application that classifies nearly 840,000 food products based on their brand and group, including the identification of the group by country for each brand. I was also asked to document my work in the form of technical documentation.

##### Implementation
To organize the project design, I chose an Excel-based methodology, where I simply followed an established schedule. To carry out this project, I had to use the Model-View-Controller (MVC) design pattern.
First, I had to install and download the missing tools needed for the project. Then, I populated a database with information about brands and groups sourced from Wikipedia.
Next, I programmed the connection and access to this database and defined the necessary functions. After that, I added a connection to the database containing the actual products. Finally, I developed the algorithm that links the products to their respective brands and groups.

##### Results
At the end of the project, I had a script capable of populating a database with brands and groups and linking the two, as well as an application that extracts products, transforms them, and sends them to the previously mentioned database to associate them with their brand and group.
The application is fully functional, except for the identification of the group by country for a brand, which has not been implemented.

### How it looks like

Here is a screenshot of the app:

<img alt="Small gif" width="100%" src="/assets/ressources/ressourceETL/App.PNG" />

### Technical documentation

Here is the technical documentation written in french

  <iframe src="/assets/ressources/ressourceETL/1_documentation_TPI.pdf#navpanes=0&toolbar=1&statusbar=1&view=Fit" width="100%" height="800px"></iframe>


### What did I learn

- **Applied the ETL (Extract, Transform, Load) process** by developing a complete pipeline to collect, clean, and store product data.

- **Used C# to build a robust application** that automates data extraction from multiple sources and interacts with both **SQL** and **NoSQL** databases.

- **Worked with MongoDB** to structure and store unstructured or semi-structured data, particularly for brand and group information.

- **Used SQL** to manage and query large datasets efficiently.

- **Implemented the MVC design pattern** to keep the application organized, modular, and maintainable.

- **Handled data integration challenges** such as associating products with their corresponding brands and groups using custom matching algorithms.

- **Populated databases programmatically** by writing scripts to fetch and process data from OpenFoodFacts and Wikipedia.

- **Learned to combine relational and non-relational databases** in a single workflow for better performance and flexibility.

- **Developed technical documentation** to track progress and clarify project architecture, decisions, and usage.

- **Improved my planning and organizational skills** by following a structured Excel-based project timeline.