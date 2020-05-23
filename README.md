# databricks-clusterimages
## A Repository to Store dockerfiles for Custom Azure Databricks Cluster Implementations

### Usage

Locate the appropriate Dockerfile that supports the use case you want to deploy then follow these steps:

    1. Change to the folder containing the Dockerfile and any needed assets
    2. Build and tag the docker container: *`docker build -t <imagename:tag>`*
    3. Push the image to dockerhub : *`docker push <imagename:tag>`*
    4. In the *Azure Portal*, navigate to your *Databricks Workspace* and launch
    5. Open the *Admin Console* and select the *Advanced* Tab
    6. Ensure that *Container Services* is Enabled
    7. Follow these instructions to deploy the image from dockerhub: https://docs.microsoft.com/en-us/azure/databricks/clusters/custom-containers