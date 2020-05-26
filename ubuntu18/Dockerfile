# Pull the bionic image from the ubuntu hub and use that as the base image
FROM ubuntu:bionic
# Make sure that the appropriate pieces for the Databricks runtimes are included
# Databricks runtime requirements are found here: https://docs.databricks.com/clusters/custom-containers.html 
# First install the JDK11

RUN apt-get update \
&& apt-get install -y openjdk-11-jdk \
&& apt-get clean;

# Fix any certificate errors
RUN apt-get update \
&& apt-get install -y ca-certificates-java \
&& apt-get clean \
&& update-ca-certificates -f;

# Ensure that the JAVA_HOME is properly set
ENV JAVA_HOME /usr/lib/jvm/java-11-openjdk-amd64/
RUN export JAVA_HOME 