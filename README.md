# k8s-elibrary-deploy

Use to deploy [eLibrary](https://github.com/johnny-butter/eLibrary) to K8S platform

## Tools

- `minikube`: standalone K8S platform
- `helm` (v3): manage deploy
- `docker-compose`: start docker-compose file

## Start Project

- Deploy to K8S (`minikube`)

```shell
helm install elibrary helm-elibrary
```

- Connect to `eLibrary` on `$(minikube ip):30080/login/`

- Check `helm` installation

```shell
helm list
```

- Remove project from K8S (`minikube`)

```shell
helm uninstall elibrary
```

## Start EFK

- `docker-compose -f docker-compose-efk.yml up`
