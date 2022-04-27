Execute Collections With Environment in Postman on Docker
This template consists of How to Execute Collections With Environment in Postman on Docker.
 
## Steps for execution

First we have to install docker on our system with the command on the terminal :-

1)sudo apt install docker.io

Now we have to pull the latest Docker image from docker hub with command :- 

2) docker pull postman/newman
  
Clone the repository

3)    

Run the command to execute postman on Docker:-

4) sudo docker run -v /home/knoldus/Desktop/Docker/collections:/etc/newman -t postman/newman:latest run     "PostmanAssignment.postman_collection.json" --environment="MyEnvironment.postman_environment.json

Technologies used

Postman , Docker

For a better understanding, please refer to the blog:- https://blog.knoldus.com/wp-admin/post.php?post=158851&action=edit