Empty ASP.NET MVC web app.

Dockerfiles:

- [Linux](dockerfile/linux.dockerfile)
- [Windows](dockerfile/windows.dockerfile) (nanoserver)

Images published to [GitHub container registry](https://github.com/users/micya/packages/container/package/webapp):

- Linux: ghcr.io/micya/webapp:linux
- Windows: ghcr.io/micya/webapp:windows

Kubernetes deployment files:

- [Linux](deployment/webapp-linux.yaml)
- [Windows](deployment/webapp-windows.yaml)

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
