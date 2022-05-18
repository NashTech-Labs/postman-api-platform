## Execute Collections with Environment on Docker

We use environment to group related sets of values together and manage access to shared Postman data if you are working as part of a team.

It is a set of variables you can use in your Postman requests. 

This template consists of How to Execute Collections With Environment in Postman on Docker. 



## Scenarios when Environment are required 

When we want to differentiate between the requests.

Change the value value of the key value pairs and the changes are reflected in our requests.

 
## Steps for execution

First we have to install docker on our system with the command on the terminal :-

1)sudo apt install docker.io

Now we have to pull the latest Docker image from docker hub with command :- 

2) docker pull postman/newman
  
Clone the repository

3) https://github.com/knoldus/postman-api-platform/tree/Execute-postman-with-environment

Run the command to execute postman on Docker:-

4) sudo docker run -v /home/knoldus/Desktop/Docker/collections:/etc/newman -t postman/newman:latest run     "PostmanAssignment.postman_collection.json" --environment="MyEnvironment.postman_environment.json"

## Techology used 

**Tool**   Postman

**Language Used** Javascript 


## For a better understanding, please refer to the blog Link :- https://blog.knoldus.com/how-to-run-postman-with-environment-on-docker/
