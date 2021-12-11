# Parameterized Jenkins Job Demo

This project was forked using the latest docker image provided by The Jenkins Continuous Integration and Delivery server [available on Docker Hub](https://hub.docker.com/r/jenkins/jenkins).

This Jenkins server is for demonstration purposes only.

NOTE: This Jenkins instance is insecure and is not production ready.

<img src="https://jenkins.io/sites/default/files/jenkins_logo.png"/>

<img src="download.png"/>

# Usage
Pull this repo

#### Log into docker
For Easy login to dockerhub.io you can set environment variables DOCKER_USERNAME and DOCKER_PASSWORD

run script
```
./.ci/common-functions.sh
```

run
```
docker pull anixdorf/jenkins
```
```
docker run -t -i -p 8080:8080 -p 50000:50000 -v ./jenkins_home:/var/jenkins_home anixdorf/jenkins
```

Your Jenkins server should be accessible at localhost:8080

For full documentation of the original docker image, please visit:
https://github.com/jenkinsci/jenkins

To download an old version of Katalon Studio that does not check for licensing, please visit: 
```https://github.com/katalon-studio/katalon-studio/releases/tag/v6.3.3```

Download the Application and start Running Tests
