# General Information
###

* AUTHOR: Eleazar Rubio Sorrentino
* EMAIL: elerubio88@gmail.com
* DESCRIPTION: Coming soon...

# Run clairctl

```
sudo docker-compose up -d

sudo docker run --rm -t                                                   /
 -v tfmdevops_reports:/go/src/github.com/jgsqware/clairctl/reports        /
 -v /var/run/docker.sock:/var/run/docker.sock:ro --net tfmdevops_default  /
 --link clair_clair:clair -p 57330:57330 tfmdevops_clairctl bash          /
 -c "cd /go/src/github.com/jgsqware/clairctl/ ;                           /
 ./clairctl analyze --log-level info --local ${DOCKER_IMAGE} ;            /
 ./clairctl report --log-level info --local ${DOCKER_IMAGE}"            

sudo docker-compose down
```