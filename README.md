# openfoam-docker-gcp
 
Running a containerized OpenFOAM in Google Cloud Platform environment (GCP). 

## Getting Started

These instructions will take you through the creation of GCP VM instance, creating and running a Docker image and running the post-installation script to test the containerized OpenFOAM installation.

### Creating a GCP VM instance

1. In the Google Cloud Console, go to the **VM instances** page.
2. Select your project and click **Continue**.
3. Click **Create instance**.
4. Specify a **Name** and **Region** for your instance.
5. Select a **Machine Type** in **Machine configuration** with 15GB memory or higher, for example, **n1-standard-4** 
6. Select a tick box **Deploy a container image to this VM instance**.
7. In the **Container image** text box, put the url (`docker.io/jiraphapa/openfoam-docker-cloud:latest`)
8. Click the **Create** button to create and start the instance.

This will create a VM instance with the Container-Optimized OS and pre-installed Docker runtime. you can access the command-line interface of an instance by ssh via the External IP address or the GCP console

### Creating and running a Docker image
