# Jenkins Data Container

## Usage
```
docker run \
--name=jenkins-data \
-v /opt/jenkins-volume/jenkins:/var/jenkins_home \
-v /opt/jenkins-volume/log:/var/log/jenkins \
samistine:jenkins-data
```

## Volumes
 * Data: ```/var/jenkins_home```
 * Logs: ```/var/log/jenkins```
 