# youtrack

![Version: 1.2.1](https://img.shields.io/badge/Version-1.2.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2023.1.16998](https://img.shields.io/badge/AppVersion-2023.1.16998-informational?style=flat-square)

A Helm chart to deploy YouTrack

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| deploymentLabels | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"jetbrains/youtrack"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/youtrack"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector."kubernetes.io/hostname" | string | `"hostname"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| selectorLabels | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| volumes[0].volume.localMountPath | string | `"/mnt/persistent/data"` |  |
| volumes[0].volume.mode | string | `"Filesystem"` |  |
| volumes[0].volume.mountPath | string | `"/opt/youtrack/data"` |  |
| volumes[0].volume.name | string | `"youtrack-data"` |  |
| volumes[0].volume.reclaimPolicy | string | `"Retain"` |  |
| volumes[0].volume.storage | string | `"10Gi"` |  |
| volumes[0].volume.storageCapacity | string | `"10Gi"` |  |
| volumes[1].volume.localMountPath | string | `"/mnt/persistent/conf"` |  |
| volumes[1].volume.mode | string | `"Filesystem"` |  |
| volumes[1].volume.mountPath | string | `"/opt/youtrack/conf"` |  |
| volumes[1].volume.name | string | `"youtrack-conf"` |  |
| volumes[1].volume.reclaimPolicy | string | `"Retain"` |  |
| volumes[1].volume.storage | string | `"1Gi"` |  |
| volumes[1].volume.storageCapacity | string | `"1Gi"` |  |
| volumes[2].volume.localMountPath | string | `"/mnt/persistent/logs"` |  |
| volumes[2].volume.mode | string | `"Filesystem"` |  |
| volumes[2].volume.mountPath | string | `"/opt/youtrack/logs"` |  |
| volumes[2].volume.name | string | `"youtrack-logs"` |  |
| volumes[2].volume.reclaimPolicy | string | `"Retain"` |  |
| volumes[2].volume.storage | string | `"2Gi"` |  |
| volumes[2].volume.storageCapacity | string | `"2Gi"` |  |
| volumes[3].volume.localMountPath | string | `"/mnt/persistent/logs"` |  |
| volumes[3].volume.mode | string | `"Filesystem"` |  |
| volumes[3].volume.mountPath | string | `"/opt/youtrack/"` |  |
| volumes[3].volume.name | string | `"youtrack-backups"` |  |
| volumes[3].volume.reclaimPolicy | string | `"Retain"` |  |
| volumes[3].volume.storage | string | `"10Gi"` |  |
| volumes[3].volume.storageCapacity | string | `"10Gi"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.3](https://github.com/norwoodj/helm-docs/releases/v1.11.3)
