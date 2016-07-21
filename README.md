# docker-ca-wekan
Kanban Practice of Wekan Image for Open DevOps Pipeline

#Usage
##docker pull  
```docker pull devopsopen/docker-ca-wekan```
##docker run : Step 1   
```docker run -d --name wekan-db devopsopen/docker-com-mongo```
##docker run : Step 2  
```docker run -d --link "wekan-db:db" -e "MONGO_URL=mongodb://db" -e "ROOT_URL=docker-host-machine-ip" -p 9090:80 devopsopen/docker-ca-wekan ```

#Web access
``` http://docker-host-machine-ip:9090 ```
