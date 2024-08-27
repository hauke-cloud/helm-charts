# fedora-coreos-images

![Version: 0.0.5](https://img.shields.io/badge/Version-0.0.5-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.5](https://img.shields.io/badge/AppVersion-0.0.5-informational?style=flat-square)

A Helm chart providing a nginx server and Fedora CoreOS images to download

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| clusterRole.create | bool | `true` |  |
| clusterRole.name | string | `""` |  |
| clusterRoleBinding.create | bool | `true` |  |
| clusterRoleBinding.name | string | `""` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/hauke-cloud/fedora-coreos-images"` |  |
| image.tag | string | `"latest"` |  |
| imagePullSecrets | list | `[]` |  |
| livenessProbe | object | `{}` |  |
| nameOverride | string | `""` |  |
| nodeSelector."node-role.kubernetes.io/control-plane" | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| readinessProbe | object | `{}` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations[0].effect | string | `"NoSchedule"` |  |
| tolerations[0].key | string | `"node-role.kubernetes.io/master"` |  |
| tolerations[0].operator | string | `"Exists"` |  |
| tolerations[1].effect | string | `"NoSchedule"` |  |
| tolerations[1].key | string | `"node-role.kubernetes.io/control-plane"` |  |
| tolerations[1].operator | string | `"Exists"` |  |
