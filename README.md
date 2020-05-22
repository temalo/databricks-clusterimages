# databricks-clusterimages
## A repository to store dockerfiles for custom Azure Databricks cluster implementations

Simple use instructions:

Locate the appropriate Dockerfile that supports the use case you want to deploy then follow these steps:
    1. Build and tag the docker container: docker build -t <imagename:tag>
    2. Push the image to dockerhub : docker push <imagename:tag>
    3. Follow the instructions here to deploy the image from dockerhub: https://docs.microsoft.com/en-us/azure/databricks/clusters/custom-containers
