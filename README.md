# databricks-clusterimages
## A Repository to Store dockerfiles for Custom Azure Databricks Cluster Implementations
### In theory these will work on AWS as well, but I have not tested that

#### Usage

Locate the appropriate Dockerfile that supports the use case you want to deploy then follow these steps:

    1. Change to the folder containing the Dockerfile and any needed assets
    2. Build and tag the docker container: _`docker build -t <imagename:tag>`_
    3. Push the image to dockerhub : _`docker push <imagename:tag>`_
    4. In the _Azure Portal_, navigate to your _Databricks Workspace_ and launch
    5. Open the _Admin Console_ and select the _Advanced_ Tab
    6. Ensure that _Container Services_ is Enabled
    7. Follow these instructions to deploy the image from dockerhub: https://docs.microsoft.com/en-us/azure/databricks/clusters/custom-containers
