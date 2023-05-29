# Prompt for manifests

| NAME | PROMPT |  DESCRIPTION  | EXAMPLE |    
|--|--|--|--|
| app.yaml | Application pod manifest | Help to deploy application - nginx, port- http:80, CPU req 0.5 lim 1, MEM req 0.5G lim 1G  | [app.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app.yaml) |
| app-livenessProbe.yaml | Service Liveness Probe | Liveness probes are a mechanism provided by Kubernetes which helps determine if applications running within containers are operational. If container not answer HTTP GET request 3 time with delay 10s, Kubernetes will restart the container.  | [app-livenessProbe.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | Service Readness Probe | Readiness probes to know when a container is ready to start accepting traffic. A readiness probe allows Kubernetes to wait 3 times of 2s until the service is active before sending it traffic. If probe failed it will be restarted due to the liveness failure.| [app-readinessProbe.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml | Service mount external storage | Application with liveness and readness probe which have external storage | [app-volumeMounts.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml | Sheduled Job | Here is a manifest for a CronJob that runs a "Hello world" task every 5 minute: | [app-cronjob.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-cronjob.yaml) |
| app-job.yaml | Job for backup | Create backup gsutil on glow-data-diks with ext4 system  | [app-job.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-job.yaml) |
| app-multicontainer.yaml | Pod with 2 containers | Creates pod with nginx and debian containers with add date in index.html every seconds. | [app-multicontainer.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-multicontainer.yaml) |
| app-resources.yaml | Describes resources which need app | Manifest describes requirements and limit of resources | [app-resources.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-resources.yaml) |
| app-secret-env.yaml | Manifest with secrets to set variables | Container sets two environment variables. | [app-secret-env.yaml](https://github.com/nirev23/new_project/blob/main/yaml/app-secret-env.yaml) |


