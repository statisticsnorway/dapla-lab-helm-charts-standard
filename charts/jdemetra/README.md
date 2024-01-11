# jdemetra

![Version: 0.0.10](https://img.shields.io/badge/Version-0.0.10-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.2.4](https://img.shields.io/badge/AppVersion-2.2.4-informational?style=flat-square)

A Helm chart for JDemetra+ with noVNC setup

**Homepage:** <https://github.com/trygu/jdemetra-docker>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Trygve Falch | <trygve.falch@gmail.com> | <https://github.com/trygu/> |

## Source Code

* <https://github.com/trygu/jdemetra-docker>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://statisticsnorway.github.io/dapla-lab-helm-charts-services | library-chart | 3.1.1 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| istio.enabled | bool | `false` |  |
| istio.gateways[0] | string | `"istio-namespace/example-gateway"` |  |
| istio.hostname | string | `"chart-example.local"` |  |
| nameOverride | string | `""` |  |
| networking.clusterIP | string | `"None"` |  |
| networking.service.port | int | `6080` |  |
| networking.type | string | `"ClusterIP"` |  |
| nodeSelector | object | `{}` |  |
| oidc.enabled | bool | `true` |  |
| oidc.secretName | string | `""` |  |
| oidc.tokenExchangeUrl | string | `""` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.enabled | bool | `false` |  |
| persistence.size | string | `"10Gi"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext.fsGroup | int | `100` |  |
| replicaCount | int | `1` |  |
| security.allowlist.enabled | bool | `false` |  |
| security.allowlist.ip | string | `"0.0.0.0/0"` |  |
| security.networkPolicy.enabled | bool | `false` |  |
| security.networkPolicy.from | list | `[]` |  |
| security.oauth2.authenticatedEmails | string | `""` |  |
| security.oauth2.clientId | string | `"my-client"` |  |
| security.oauth2.oidcIssuerUrl | string | `""` |  |
| security.oauth2.provider | string | `"keycloak-oidc"` |  |
| security.password | string | `"changeme"` |  |
| security.serviceEntry.enabled | bool | `true` |  |
| security.serviceEntry.hosts | list | `[]` |  |
| securityContext | object | `{}` |  |
| service.image.pullPolicy | string | `"IfNotPresent"` |  |
| service.image.version | string | `"trygu/nbdemetra:0.7"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)