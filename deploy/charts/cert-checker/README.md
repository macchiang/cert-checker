# cert-checker

![Version: 0.0.2](https://img.shields.io/badge/Version-0.0.2-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.0.2](https://img.shields.io/badge/AppVersion-v0.0.2-informational?style=flat-square)

A tool to expose SSL Certificate information as prometheus metrics.

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| certchecker.certificates[0].dns | string | `"google.com"` |  |
| certchecker.certificates[10].dns | string | `"null.badssl.com"` |  |
| certchecker.certificates[11].dns | string | `"rc4-md5.badssl.com"` |  |
| certchecker.certificates[12].dns | string | `"rc4.badssl.com"` |  |
| certchecker.certificates[1].dns | string | `"example.com"` |  |
| certchecker.certificates[2].dns | string | `"twitter.com"` |  |
| certchecker.certificates[3].dns | string | `"expired.badssl.com"` |  |
| certchecker.certificates[4].dns | string | `"wrong.host.badssl.com"` |  |
| certchecker.certificates[5].dns | string | `"untrusted-root.badssl.com"` |  |
| certchecker.certificates[6].dns | string | `"self-signed.badssl.com"` |  |
| certchecker.certificates[7].dns | string | `"revoked.badssl.com"` |  |
| certchecker.certificates[8].dns | string | `"dh480.badssl.com"` |  |
| certchecker.certificates[9].dns | string | `"dh512.badssl.com"` |  |
| certchecker.intervalminutes | int | `1` |  |
| certchecker.loglevel | string | `"info"` |  |
| fullnameOverride | string | `""` |  |
| grafanaDashboard.enabled | bool | `false` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"mogensen/cert-checker"` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations."enable.cert-checker.io/cert-checker" | string | `"true"` |  |
| podAnnotations."prometheus.io/path" | string | `"/metrics"` |  |
| podAnnotations."prometheus.io/port" | string | `"8080"` |  |
| podAnnotations."prometheus.io/scrape" | string | `"true"` |  |
| podSecurityContext.fsGroup | int | `2000` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext.allowPrivilegeEscalation | bool | `false` |  |
| securityContext.capabilities.drop[0] | string | `"ALL"` |  |
| securityContext.privileged | bool | `false` |  |
| securityContext.readOnlyRootFilesystem | bool | `true` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `1000` |  |
| service.port | int | `8080` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| serviceMonitor.additionalLabels | object | `{}` |  |
| serviceMonitor.enabled | bool | `false` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)