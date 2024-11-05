Hi, this is Krishna Pavani Damaraparapu. This repo is a part of my Mini-Project does for my academics. I have choose this TODO project and build Pipelines to deploy the app to an EC2 instance on AWS. The workflow connects to an AWS account via Access Key and creates infrastructure - VPC, Internetgateway, Subnet, Security Groups and an EC2 instance. It then runs deployment commands inside of the instance using the Public IP and the SSH key attached to it.
___
A demonstration of Docker to implement a simple 3 tier architecture

* frontend will be able to access the mid-tier
* mid-tier will be able to access the db

In order to run this in docker, simply type ```docker-compose up``` at the command prompt. Docker will then create the [MongoDB](https://www.mongodb.com/) from the stock [mongo](https://hub.docker.com/_/mongo) image. The api uses [nodejs](https://nodejs.org/) with [express](http://expressjs.com/) and is built from a [node:alpine](https://hub.docker.com/_/node) image. The front end uses [ReactJS](https://reactjs.org/) and built from a [node:alpine](https://hub.docker.com/_/node) image.
