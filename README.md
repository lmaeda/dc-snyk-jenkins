# dc-snyk-jenkins
docker-compose level app to check out the latest of Jenkins and Snyk for CI pipeline

docker run --name myjenkins --rm --publish 8080:8080 --publish 50000:50000 --volume /var/run/docker.sock:/var/run/docker.sock:rw --volume jenkins-data:/var/jenkins_home --volume jenkins-docker-certs:/certs/client:ro --volume "$HOME":/home --env JENKINS_ADMIN_ID=${JENKINS_ADMIN_ID} --env JENKINS_ADMIN_PASSWORD=${JENKINS_ADMIN_PASSWORD} lucmaeda:myjcasc
