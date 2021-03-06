# nginx

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.19.0](https://img.shields.io/badge/AppVersion-1.19.0-informational?style=flat-square)

Nginx Helm chart for Kubernetes

## Requirements
* [mysql](https://github.com/krakazyabra/microservices/wiki/Databases)

## Dependencies

| Repository | Name | Version |
|------------|------|---------|
| https://krakazyabra.github.io/microservices/ | common | ~0.1.13 |

## TL;DR
```console
$ helm repo add krakazyabra https://krakazyabra.github.io/microservices/
$ helm repo update
$ helm install nginx krakazyabra/nginx
```

## Installing the Chart
To install the chart with the release name `nginx`:
```console
helm install nginx krakazyabra/nginx
```

## Uninstalling the Chart
To uninstall the `nginx` deployment:
```console
helm uninstall nginx
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.
Other values may be used from the [values.yaml](../common/values.yaml) from the [common library](../common).

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install nginx \
  --set env.TZ="America/New York" \
    krakazyabra/nginx
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install nginx krakazyabra/nginx -f values.yaml
```

## Troubleshooting
See [Wiki](https://github.com/krakazyabra/microservices/wiki/Troubleshooting).

## Author
This project was started in 2021 by [Egor Pronin](https://github.com/krakazyabra).

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.4.0](https://github.com/norwoodj/helm-docs/releases/v1.4.0)
