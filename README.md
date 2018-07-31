# Business Intelligence and Data Warehouse Course

This repository contains all necessary inputs to run the course hands-on labs. 

## Repository contents (by session)

  - Additional articles and documents
  - MySQL Workbench Schemas
  - ETL processes
  - Datasets
  - Tableau files
  - Videos

## Software Installation

  - **Data Warehouse**: MySQL (database) and MySQL Workbench (database modeling and SQL development)
  - **ETL**: Pentaho Data Integration (PDI)
  - **Business Intelligence/Data Visualization**: Tableau Desktop
  - **Self-Service of Data Lakes**: Dremio

### Steps

**Install Java**

  - Download Java JDK v8 from: http://www.oracle.com/technetwork/java/javase/downloads/index-jsp-138363.html (in our case: Java SE 8u171/8u172)
  - Install and follow the instructions

**Install MySQL**

  - Download the right version of MySQL and MySQL Workbench for your OS (in our case: MySQL Community Server 8.0.12 and MySQL Workbench 8.0.12) 
    - MySQL: http://dev.mysql.com/downloads/mysql/
    - MySQL Workbench: http://dev.mysql.com/downloads/workbench/
  - Install all the programs and follow the instructions:
    - [Windows] During the installation process you will configure the password for root user (choose pentaho2018 o a password that you will remember).
    - [Mac] During the installation process you will configure the password for root user (choose pentaho2018 o a password that you will remember). If you forget the password you will be able to change it from system preferences.
    - PDI and MySQL Workbench only supports legacy password encription, not the new strong encription available in MySQL 8.

> Note: for Microsoft Windows it is just one installer for MAC, two files.

Remember to start the server to be able to use the database. Open MySQL Workbench and create a new connection using the right user and password and the standard parameters for configuration.

**Install PDI**

We will use the community version of Pentaho Data Integration (a.k.a PDI). It can be downloaded from this [link](https://sourceforge.net/projects/pentaho/files/Pentaho%208.1/client-tools/) (in our case: pdi-ce-8.1.0.0-65.zip).

  - Download the file and unzip.
    - [Mac] Move the data-integration folder into Applications folder
    - [Windows] Move the data-integration folder into C:/ folder
  - Open PDI
    - [Windows] Double-click spoon.bat inside data-integratioon folder
    - [Mac] Open the terminal and execute:
    
```
cd /Applications/data-integration/
./spoon.sh
```    
  - [Optional] Activate data-integration.app as a double-click app using the terminal:
  
``` 
sudo xattr -dr com.apple.quarantine /Applications/data-integration/Data\ Integration.app
```  

  - Install MySQL plugin for PDI:
    - Open PDI
    - Go the tools menu > Marketplace > MySQL Plugin and install
    - Restart PDI

**Install Tableau Desktop**

We can access student licenses due to the Academic Partnership. Tableau has versions for Mac and Windows. Follow these instructions:

  - Download the latest version of Tableau Desktop [here](https://www.tableau.com/academic).
  - Copy Tableau Desktop License from campus.
  - Install the software following the instructions in the screen.
  - Update your license in the application: Help menu -> Manage Product Keys

**Install Dremio**

We will use the community version of Dremio Server. It can be downloaded from this [link](https://www.dremio.com/download/). Dremio server requires Java to work. Then:

  - Install Dremio using the installer.
  - Start Dremio:
      - [Windows]: Start from the Start Menu.
      - [Mac]: Launch Dremio from Applications. Start Dremio from the Start Menu.
  - You can now navigate to the Dremio UI at http://localhost:9047.

## FAQ

### Is there a Pentaho Release Product Version Matrix?

Yes! You can find it [here](https://wiki.pentaho.com/display/PEOpen/Pentaho+Release+Product+Version+Matrix+8.x).

### Any recommendation for MySQL SQL syntax?

Yes, check [MySQL™ Notes for Professionals book](http://books.goalkicker.com/MySQLBook/) and [MySQL Documentation](https://dev.mysql.com/doc/).

### How can I have this repository?

Fork it using [github](https://www.github.com) and [github desktop](https://www.desktop.github.com).
