This is an automated instalation of jenkins using docker

Follow steps below to run the jenkins server

1 - build the image: 

docker build . -t jenkins:jcasc

2 - Run the container

docker run -d --name jenkins --rm -p 8080:8080 --env JENKINS_ADMIN_ID=admin --env JENKINS_ADMIN_PASSWORD=admin jenkins:jcasc

3 - Wait for jenkins to start
4 - Log in with the admin password provided

This repository implements a jenkins server as described in the page below:
https://www.digitalocean.com/community/tutorials/how-to-automate-jenkins-setup-with-docker-and-jenkins-configuration-as-code