# Usage

To run Terraform commands, you can mount your project in a volume under `/app`. 

```
docker run -ti --rm -v $PWD:/app 1science/python-sonar:3.6 sonar-scanner \
     -Dsonar.projectKey=<project-key> \
     -Dsonar.organization=<org> \
     -Dsonar.sources=. \
     -Dsonar.host.url=https://sonarcloud.io \
     -Dsonar.login=<token>
```

# Build

This project is configured as an [automated build in Dockerhub](https://hub.docker.com/r/1science/python-sonar/).

Each branch give the related image tag.  

# License

All the code contained in this repository, unless explicitly stated, is
licensed under ISC license.

A copy of the license can be found inside the [LICENSE](LICENSE) file.