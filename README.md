# jenkins

Installation: Running the container

After you have installed docker, run following to get Jenkins up and running.

    docker run -it -p 8080:8080 -p 50000:50000 \
	    -v jenkins_home:/var/jenkins_home \
	    -v /var/run/docker.sock:/var/run/docker.sock \
	    --restart unless-stopped \
	    4oh4/jenkins-docker
