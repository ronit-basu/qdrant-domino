# qdrant

![Version: 0.7.4-0.0.1](https://img.shields.io/badge/Version-0.7.4--0.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v1.7.3](https://img.shields.io/badge/AppVersion-v1.7.3-informational?style=flat-square)

Qdrant - Vector Database for the next generation of AI applications.

## Source Code

* <https://github.com/qdrant/qdrant>
* <https://github.com/qdrant/qdrant-helm>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| oci://gcr.io/domino-eng-service-artifacts | commonlib | 0.13.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalLabels | object | `{}` |  |
| additionalVolumeMounts | list | `[]` |  |
| additionalVolumes | list | `[]` |  |
| affinity | object | `{}` |  |
| apiKey | bool | `true` |  |
| args[0] | string | `"./config/initialize.sh"` |  |
| config.cluster.consensus.tick_period_ms | int | `100` |  |
| config.cluster.enabled | bool | `true` |  |
| config.cluster.p2p.port | int | `6335` |  |
| config.service.enable_tls | bool | `false` |  |
| containerSecurityContext.allowPrivilegeEscalation | bool | `false` |  |
| containerSecurityContext.privileged | bool | `false` |  |
| containerSecurityContext.readOnlyRootFilesystem | bool | `true` |  |
| containerSecurityContext.runAsGroup | int | `2000` |  |
| containerSecurityContext.runAsNonRoot | bool | `true` |  |
| containerSecurityContext.runAsUser | int | `1000` |  |
| env | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"docker.io/qdrant/qdrant"` |  |
| image.tag | string | `""` |  |
| image.useUnprivilegedImage | bool | `false` |  |
| imagePullSecrets | list | `[]` |  |
| livenessProbe.enabled | bool | `false` |  |
| livenessProbe.failureThreshold | int | `6` |  |
| livenessProbe.initialDelaySeconds | int | `5` |  |
| livenessProbe.periodSeconds | int | `5` |  |
| livenessProbe.successThreshold | int | `1` |  |
| livenessProbe.timeoutSeconds | int | `1` |  |
| metrics.serviceMonitor.additionalLabels | object | `{}` |  |
| metrics.serviceMonitor.enabled | bool | `false` |  |
| metrics.serviceMonitor.metricRelabelings | list | `[]` |  |
| metrics.serviceMonitor.relabelings | list | `[]` |  |
| metrics.serviceMonitor.scrapeInterval | string | `"30s"` |  |
| metrics.serviceMonitor.scrapeTimeout | string | `"10s"` |  |
| metrics.serviceMonitor.targetPath | string | `"/metrics"` |  |
| metrics.serviceMonitor.targetPort | string | `"http"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| persistence.annotations | object | `{}` |  |
| persistence.size | string | `"10Gi"` |  |
| podAnnotations | object | `{}` |  |
| podDisruptionBudget.enabled | bool | `false` |  |
| podDisruptionBudget.maxUnavailable | int | `1` |  |
| podDisruptionBudget.unhealthyPodEvictionPolicy | string | `""` |  |
| podLabels | object | `{}` |  |
| podSecurityContext.fsGroup | int | `3000` |  |
| podSecurityContext.fsGroupChangePolicy | string | `"Always"` |  |
| priorityClassName | string | `""` |  |
| readinessProbe.enabled | bool | `true` |  |
| readinessProbe.failureThreshold | int | `6` |  |
| readinessProbe.initialDelaySeconds | int | `5` |  |
| readinessProbe.periodSeconds | int | `5` |  |
| readinessProbe.successThreshold | int | `1` |  |
| readinessProbe.timeoutSeconds | int | `1` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| service.additionalLabels | object | `{}` |  |
| service.annotations | object | `{}` |  |
| service.ports[0].checksEnabled | bool | `true` |  |
| service.ports[0].name | string | `"http"` |  |
| service.ports[0].port | int | `6333` |  |
| service.ports[0].protocol | string | `"TCP"` |  |
| service.ports[0].targetPort | int | `6333` |  |
| service.ports[1].checksEnabled | bool | `false` |  |
| service.ports[1].name | string | `"grpc"` |  |
| service.ports[1].port | int | `6334` |  |
| service.ports[1].protocol | string | `"TCP"` |  |
| service.ports[1].targetPort | int | `6334` |  |
| service.ports[2].checksEnabled | bool | `false` |  |
| service.ports[2].name | string | `"p2p"` |  |
| service.ports[2].port | int | `6335` |  |
| service.ports[2].protocol | string | `"TCP"` |  |
| service.ports[2].targetPort | int | `6335` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| sidecarContainers | list | `[]` |  |
| snapshotRestoration.enabled | bool | `false` |  |
| snapshotRestoration.pvcName | string | `"snapshots-pvc"` |  |
| snapshotRestoration.snapshots | string | `nil` |  |
| startupProbe.enabled | bool | `false` |  |
| startupProbe.failureThreshold | int | `30` |  |
| startupProbe.initialDelaySeconds | int | `10` |  |
| startupProbe.periodSeconds | int | `5` |  |
| startupProbe.successThreshold | int | `1` |  |
| startupProbe.timeoutSeconds | int | `1` |  |
| tolerations | list | `[]` |  |
| topologySpreadConstraints | list | `[]` |  |
| updateConfigurationOnChange | bool | `false` |  |
| updateVolumeFsOwnership | bool | `true` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.2](https://github.com/norwoodj/helm-docs/releases/v1.11.2)
