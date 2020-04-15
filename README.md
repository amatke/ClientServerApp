# Client - Server application using socket

### Calling the Application

Command example for launching the server application with 3 different parameters:
1) **java –jar server_2.jar portNumber pathToDataBase pathToOutputDir**
* **portNumber** - Integer value representing the number of the port on which the server listens
* **pathToDatabase** – String that contains the path to the sqlite3 database file (e.g. ./inputDir/database.sqlite3). The SQLite file will always be provided
* **pathToOutputDir** – String that contains path to specific output location where zip file should be stored

After the server application, you can launch the client application:
2) **java –jar client_2.jar serverAddress portNumber pathToInputDir**
* **serverAddress** – String that describes the server computer address
* **portNumber** - Integer value representing the port number on which the application will expect requests
* **pathToInputDir** – String that contains the path to the input directory (e.g. ./input/path/inputDir). The input directory will always be provided. This directory will contain one or more input files whose format might be excel, text… (.xlsx, .txt)
