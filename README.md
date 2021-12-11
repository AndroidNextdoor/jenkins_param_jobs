<img src="https://jenkins.io/sites/default/files/jenkins_logo.png"/>

# Jenkins Parameterized Katalon Job
## Use the power of Katalon Studio's easy record, startup and go approach with the power of Jenkins automation and get instant results in software testing.

This project was forked using the latest docker image provided by The Jenkins Continuous Integration and Delivery server [available on Docker Hub](https://hub.docker.com/r/jenkins/jenkins).

This Jenkins server is for demonstration purposes only. Many parameter plugins were applied to the instance.

!! This Jenkins instance is insecure and is not production ready - Use at your own risk. I've installed the jenkins plugin "skip-certificate-check" to the docker image. Remove that plugin and install certs correctly if necessary  !!

##Visit Jenkins.io
###Jenkins is a fantastic tool! It is used by many organizations because it's easy to use.

##Pull this repo 

For easy authentication to dockerhub.io, you can set environment variables DOCKER_USERNAME and DOCKER_PASSWORD

On a Mac or linux OS run these commands to log in to docker and start up a local instance
```
./.ci/common-functions.sh

docker pull anixdorf/jenkins

docker run -t -i -p 8080:8080 -p 50000:50000 -v ./jenkins_home:/var/jenkins_home anixdorf/jenkins
```

Your Jenkins server should be accessible at localhost:8080

For full documentation of the original docker image, please visit:
https://github.com/jenkinsci/jenkinsK

![Katalon](download.png) 
##Visit Katalon.com

I love their approach to testing. Works as an excellent Blackbox approach to testing.

To download an old opensource version of Katalon Studio that does not check for licensing, please visit: 
```https://github.com/katalon-studio/katalon-studio/releases/tag/v6.3.3```

Download and start running parameterized Katalon <3 Jenkins tests in no time. Excellent in a CI/CD pipeline.


