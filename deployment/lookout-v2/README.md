# armada-lookout-v2

![Version: LATEST](https://img.shields.io/badge/Version-LATEST-informational?style=flat-square) ![AppVersion: LATEST](https://img.shields.io/badge/AppVersion-LATEST-informational?style=flat-square)

A helm chart for Armada Lookout component

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalLabels | object | `{}` |  |
| applicationConfig.grpcPort | int | `50051` |  |
| applicationConfig.httpPort | int | `8080` |  |
| applicationConfig.metricsPort | int | `9000` |  |
| customServiceAccount | string | `nil` |  |
| image.repository | string | `"gresearchdev/armada-lookout"` |  |
| image.tag | string | `"LATEST"` |  |
| ingress.annotations | object | `{}` |  |
| ingress.labels | object | `{}` |  |
| prometheus.enabled | bool | `false` |  |
| prometheus.labels | object | `{}` |  |
| prometheus.scrapeInterval | string | `"10s"` |  |
| replicas | int | `1` |  |
| resources.limits.cpu | string | `"300m"` |  |
| resources.limits.memory | string | `"1Gi"` |  |
| resources.requests.cpu | string | `"200m"` |  |
| resources.requests.memory | string | `"512Mi"` |  |
| serviceAccount | string | `nil` |  |
| strategy.rollingUpdate.maxUnavailable | int | `1` |  |
| strategy.type | string | `"RollingUpdate"` |  |
| terminationGracePeriodSeconds | int | `5` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)