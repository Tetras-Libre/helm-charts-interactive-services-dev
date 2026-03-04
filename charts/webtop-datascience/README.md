# webtop-data-science

![Version: 0.0.34](https://img.shields.io/badge/Version-0.0.34-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square)

Webtop VNC for data science

**Homepage:** <https://docs.linuxserver.io/images/docker-webtop/>

## Source Code

* <https://github.com/InseeFrLab/images-datascience>
* <https://github.com/Tetras-Libre/helm-charts-interactive-services>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://inseefrlab.github.io/helm-charts-interactive-services | library-chart | 1.7.13 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalVolumeMounts | list | `[]` |  |
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| certificates | object | `{}` |  |
| chromadb.secretName | string | `""` |  |
| coresite.secretName | string | `""` |  |
| discovery.chromadb | bool | `true` |  |
| discovery.hive | bool | `true` |  |
| discovery.metaflow | bool | `true` |  |
| discovery.milvus | bool | `true` |  |
| discovery.mlflow | bool | `true` |  |
| discovery.postgresql | bool | `true` |  |
| environment.CUSTOM_USER | string | `"onyxia"` |  |
| environment.group | string | `"users"` |  |
| extraEnvVars | list | `[]` |  |
| fullnameOverride | string | `""` |  |
| git.branch | string | `""` |  |
| git.cache | string | `""` |  |
| git.email | string | `""` |  |
| git.enabled | bool | `false` |  |
| git.name | string | `""` |  |
| git.repository | string | `""` |  |
| git.secretName | string | `""` |  |
| git.token | string | `""` |  |
| global.suspend | bool | `false` |  |
| hive.secretName | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations."traefik.ingress.kubernetes.io/router.tls.certresolver" | string | `"myresolver"` |  |
| ingress.certManagerClusterIssuer | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hostname | string | `"chart-example.local"` |  |
| ingress.ingressClassName | string | `""` |  |
| ingress.path | string | `"/"` |  |
| ingress.tls | bool | `true` |  |
| ingress.tlsSecretName | string | `""` |  |
| ingress.useCertManager | bool | `false` |  |
| ingress.useTlsSecret | bool | `false` |  |
| ingress.userHostname | string | `"chart-example-user.local"` |  |
| ingress.userPath | string | `"/"` |  |
| init.personalInit | string | `""` |  |
| init.personalInitArgs | string | `""` |  |
| init.regionInit | string | `""` |  |
| init.standardInitPath | string | `"/init"` |  |
| kubernetes.enabled | bool | `false` |  |
| kubernetes.role | string | `"view"` |  |
| message.en | string | `""` |  |
| message.fr | string | `""` |  |
| metaflow.secretName | string | `""` |  |
| milvus.secretName | string | `""` |  |
| mlflow.secretName | string | `""` |  |
| nameOverride | string | `""` |  |
| networking.clusterIP | string | `"None"` |  |
| networking.service.port | int | `3000` |  |
| networking.type | string | `"ClusterIP"` |  |
| networking.user.enabled | bool | `false` |  |
| networking.user.port | int | `3000` |  |
| networking.user.ports | list | `[]` |  |
| nodeSelector | object | `{}` |  |
| openshiftSCC.enabled | bool | `false` |  |
| openshiftSCC.scc | string | `""` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.enabled | bool | `false` |  |
| persistence.size | string | `"10Gi"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext.fsGroup | int | `100` |  |
| postgresql.secretName | string | `""` |  |
| proxy.enabled | bool | `false` |  |
| proxy.httpProxy | string | `""` |  |
| proxy.httpsProxy | string | `""` |  |
| proxy.noProxy | string | `""` |  |
| replicaCount | int | `1` |  |
| repository.condaRepository | string | `""` |  |
| repository.configMapName | string | `""` |  |
| repository.pipRepository | string | `""` |  |
| resources | object | `{}` |  |
| route.annotations | list | `[]` |  |
| route.enabled | bool | `false` |  |
| route.hostname | string | `"chart-example.local"` |  |
| route.tls.termination | string | `"edge"` |  |
| route.userHostname | string | `"chart-example-user.local"` |  |
| route.wildcardPolicy | string | `"None"` |  |
| s3.accessKeyId | string | `""` |  |
| s3.defaultRegion | string | `""` |  |
| s3.enabled | bool | `false` |  |
| s3.endpoint | string | `""` |  |
| s3.pathStyleAccess | bool | `false` |  |
| s3.secretAccessKey | string | `""` |  |
| s3.secretName | string | `""` |  |
| s3.sessionToken | string | `""` |  |
| s3.workingDirectoryPath | string | `""` |  |
| security.allowlist.enabled | bool | `false` |  |
| security.allowlist.ip | string | `"0.0.0.0/0"` |  |
| security.networkPolicy.enabled | bool | `false` |  |
| security.networkPolicy.from | list | `[]` |  |
| security.password | string | `"changeme"` |  |
| securityContext.capabilities.add[0] | string | `"CHOWN"` |  |
| securityContext.capabilities.add[1] | string | `"SETUID"` |  |
| securityContext.capabilities.add[2] | string | `"SETGID"` |  |
| securityContext.capabilities.drop[0] | string | `"ALL"` |  |
| securityContext.readOnlyRootFilesystem | bool | `false` |  |
| securityContext.runAsGroup | int | `0` |  |
| securityContext.runAsNonRoot | bool | `false` |  |
| securityContext.runAsUser | int | `0` |  |
| service.image.custom.enabled | bool | `false` |  |
| service.image.custom.version | string | `"tetraslibre/kasm-data-science:latest"` |  |
| service.image.pullPolicy | string | `"Always"` |  |
| service.image.version | string | `"tetraslibre/kasm-data-science:latest"` |  |
| service.initContainer.image | string | `"tetraslibre/kasm-data-science:latest"` |  |
| service.initContainer.pullPolicy | string | `"IfNotPresent"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| startupProbe.failureThreshold | int | `60` |  |
| startupProbe.initialDelaySeconds | int | `10` |  |
| startupProbe.periodSeconds | int | `10` |  |
| startupProbe.successThreshold | int | `1` |  |
| startupProbe.timeoutSeconds | int | `2` |  |
| tolerations | list | `[]` |  |
| userPreferences.aiAssistant.apiBase | string | `""` |  |
| userPreferences.aiAssistant.apiKey | string | `""` |  |
| userPreferences.aiAssistant.embeddingsProvider | string | `""` |  |
| userPreferences.aiAssistant.enabled | bool | `false` |  |
| userPreferences.aiAssistant.modelProvider | string | `""` |  |
| userPreferences.aiAssistant.secretName | string | `""` |  |
| userPreferences.darkMode | bool | `false` |  |
| userPreferences.language | string | `"en"` |  |
| vault.directory | string | `""` |  |
| vault.enabled | bool | `false` |  |
| vault.mount | string | `""` |  |
| vault.secret | string | `""` |  |
| vault.secretName | string | `""` |  |
| vault.token | string | `""` |  |
| vault.url | string | `""` |  |
| volumes | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
