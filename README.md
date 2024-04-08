Overview
--------
This project demonstrates how to develop an Azure Fuctions app in Java.
The project was created with Azure Functions Core Tools using
```
func init
func new
``` 

Building
--------
To build this project, use Maven:
```
mvn build
```

Running
-------
To run the app using a local Azure Functions host, do the following: 
1) download and install Azure Functions Core Tools 
2) execute below command to start the host and launch the app in it:
```
mvn azure-functions:run
``` 

You should see output similar to be the below:
```
[2024-04-08T09:38:57.539Z] Worker process started and initialized.

Functions:

        HttpExample: [GET,POST] http://localhost:7071/api/HttpExample
```

Now you can send HTTP GET and POST requests to the HTTP end-point using curl or a web browser.

References
----------
- https://learn.microsoft.com/en-us/azure/azure-functions/functions-run-local?tabs=linux%2Cisolated-process%2Cnode-v4%2Cpython-v2%2Chttp-trigger%2Ccontainer-apps&pivots=programming-language-java