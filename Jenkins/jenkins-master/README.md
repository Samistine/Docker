# Jenkins Master Container

## Usage
```
sudo docker run -p 127.0.0.1:8080:8080 \
--name=jenkins-master \
--volumes-from=jenkins-data \
-d \
--restart="always" \
samistine\jenkins-master
```

## Optional Parameters
 * `-e TZ=America/New_York`
 * `-e JAVA_OPTS="-Xmx8192m"`
 * `-e JENKINS_JAVA_OPTIONS="-Duser.timezone=America/New_York"`
 * `-e JENKINS_OPTS="--handlerCountStartup=100 --handlerCountMax=300 --logfile=/var/log/jenkins/jenkins.log  --webroot=/var/cache/jenkins/war"`
 