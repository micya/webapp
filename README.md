Empty ASP.NET MVC web app.

Dockerfiles:

- [Linux](dockerfiles/linux.dockerfile)
- [Windows](dockerfiles/windows.dockerfile) (nanoserver)

Images published to [DockerHub](https://hub.docker.com/repository/docker/micya/webapp/general):

- Linux: micya/webapp:linux
- Windows: micya/webapp:windows

Kubernetes deployment files:

- [Linux](deployments/webapp-linux.yaml)
- [Windows](deployments/webapp-windows.yaml)

Helm charts:
- [Linux](charts/webapp-linux)
- [Windows](charts/webapp-windows)
