# sulfoxide-xenon

![Version: 1.12.0](https://img.shields.io/badge/Version-1.12.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 3.12.1](https://img.shields.io/badge/AppVersion-3.12.1-informational?style=flat-square)

Metrics Server

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://kubernetes-sigs.github.io/metrics-server/ | metrics-server | 3.12.1 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| metrics-server | object | `{"commonLabels":{"<<":{"atomi.cloud/layer":"1","atomi.cloud/module":"operator","atomi.cloud/platform":"sulfoxide","atomi.cloud/service":"xenon"}},"podAnnotations":{"<<":{"atomi.cloud/layer":"1","atomi.cloud/module":"operator","atomi.cloud/platform":"sulfoxide","atomi.cloud/service":"xenon"}},"serviceMonitor":{"enabled":true},"topologySpreadConstraints":[{"labelSelector":{"matchLabels":{"<<":{"atomi.cloud/layer":"1","atomi.cloud/module":"operator","atomi.cloud/platform":"sulfoxide","atomi.cloud/service":"xenon"}}},"maxSkew":1,"topologyKey":"topology.kubernetes.io/zone","whenUnsatisfiable":"ScheduleAnyway"}]}` | Metrics Server Configuration. See the [Helm Chart documentation](https://kubernetes-sigs.github.io/metrics-server/) |
| serviceTree | object | `{"layer":"1","module":"operator","platform":"sulfoxide","service":"xenon"}` | AtomiCloud Service Tree. See [ServiceTree](https://atomicloud.larksuite.com/wiki/OkfJwTXGFiMJkrk6W3RuwRrZs64?theme=DARK&contentTheme=DARK#MHw5d76uDo2tBLx86cduFQMRsBb) |
| tags | object | `{"atomi.cloud/layer":"1","atomi.cloud/module":"operator","atomi.cloud/platform":"sulfoxide","atomi.cloud/service":"xenon"}` | Kubernetes labels and annotations, following Service Tree |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
