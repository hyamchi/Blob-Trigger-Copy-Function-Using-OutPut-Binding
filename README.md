# Blob-Triggered-Azure-Function
This function gets triggered when a new blob is created in the source container and makes a copy of the new blob in the destination container with the help of output binding. 

# Local Testing:
You should have a `local.settings.json` file in the root dir of the project and specify the values for connection strings and AzurewebJobsStorage:
![Untitled](https://user-images.githubusercontent.com/84933778/187780332-92acc1db-095f-406e-9e74-99cf83dd60f1.png)

To get the connection string for an Azure Storage Account go to the storage account and from the left pane select “Access Keys” and then click on “Show” and copy the value.
![Untitled1](https://user-images.githubusercontent.com/84933778/187779260-a68254d2-00e7-4cac-9b54-14b75e5068dc.png)
# Testing The Function in Azure:
To test the function in Azure, you need to store the connection values in the Function App's `Application Settings`:
![Untitled3](https://user-images.githubusercontent.com/84933778/187781361-e9f60fc0-0c82-4eb9-9df1-43253145da96.png)

For more info refer to the following links:

https://docs.microsoft.com/en-us/azure/azure-functions/functions-bindings-storage-blob-output?tabs=in-process%2Cextensionv5&pivots=programming-language-python

https://docs.microsoft.com/en-us/azure/azure-functions/functions-bindings-storage-blob-input?tabs=in-process%2Cextensionv5&pivots=programming-language-python
