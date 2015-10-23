# Ghost Standalone Docker-Compose Installation
This is a simple docker-compose ghost project that allows you to quickly get up and running with Ghost and volumes mounted to the host so you can store your theme, images, and databases locally.

## Why is this Ghost project different?
Wrapping Ghost into a Docker compose file automatically injects alot more funtionality. We will build upon this project to build High Availability, seperate data containers, and finally continous deployment and continuous integration

## Getting started
Before you get started be sure to install the latest versions of docker engine and docker-compose. Next clone this repo to your docker host and follow the configuration steps below.

## Configuration
* Edit the docker-compose.yml with your project information (URL, Host Directory Paths, etc)
* Edit the [config.js](https://github.com/vegasbrianc/Ghost-Standalone/blob/master/ghost/config.js) with your database paths in the database section in both Production and Development sections 
* Edit the [Dockerfile](https://github.com/vegasbrianc/Ghost-Standalone/blob/master/ghost/Dockerfile) with your URL information

## Start it up
Once you've edited the configuration files you are ready to get started.  Run the below command which will build your Ghost blog.

    docker-compose up
