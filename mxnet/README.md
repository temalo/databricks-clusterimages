This folder contains the dockerfile that can be used to create a new cluster image that is based on the dbruntime:standard base
image (which is based on ubuntu xenial (16.04) and includes the databricks standard runtime)
This includes an installation for Microsoft R Open 3.5.3 and provides various updates
This also includes various updates to packages that are required to build and install MxNet
Apache MxNet (currently incubating) is downloaded, built, and installed. 
Language extensions are added for both R and Python.
The result is a container image that can be deployed to Azure Databricks using the custom container deployment options
found here: https://docs.microsoft.com/en-us/azure/databricks/clusters/custom-containers
The recommendation is to push the docker image to dockerhub and deploy from there
