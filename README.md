# DockerCI

Build the image with:

```bash
docker build -t leofaber/ci:jenkins_singularity .
```

Run the container with:
```bash
docker run -d -u root --privileged --name CI_jenkins_singularity -v jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock -p 8080:8080 -p 50000:50000 leofaber/ci:jenkins_singularity
```

The image is hosted here https://hub.docker.com/r/leofaber/ci/
