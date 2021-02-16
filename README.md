Empty ASP.NET MVC web app.

Dockerfiles:

- [Linux](dockerfile/linux.dockerfile)
- [Windows](dockerfile/windows.dockerfile) (nanoserver)

Images published to [GitHub container registry](https://github.com/users/micya/packages/container/package/webapp).

Deploy via Kubernetes [deployment file](deployment/webapp.yaml) as below:

```bash
# if repo was cloned
kubectl apply -f deployment/webapp.yaml

# if repo was not cloned
kubectl apply -f https://raw.githubusercontent.com/micya/webapp/master/deployment/webapp.yaml
```

Deploy via [helm chart](charts/webapp) as below:

```bash
# add repo
helm repo add webapp https://raw.githubusercontent.com/micya/webapp/master/charts
helm repo update

# install helm chart
helm install webapp webapp/webapp
```
