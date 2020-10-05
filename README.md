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

Deploy helm chart as below:

```bash
# add repo
helm repo add webapp https://raw.githubusercontent.com/micya/webapp/master/charts
# install linux helm chart
helm install webapp-linux webapp/webapp-linux
# install windows helm chart
helm install webapp-windows webapp/webapp-windows
```
