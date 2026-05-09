# ChatGPT yaml prompt for DevOps

|NAME|PROMPT|DESCRIPTION|EXAMPLE|
|--|--|--|--|
|app.yaml|Create app.yaml, apiVersion: v1 and kind: Pod|App Engine app's settings|[app.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app.yaml)|
|app-livenessProbe.yaml|Create app-livenessProbe.yaml based on the app.yaml above|The kubelet uses liveness probes to know when to restart a container|[app-livenessProbe.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-livenessProbe.yaml)|
|app-readinessProbe.yaml|Create app-readinessProbe.yaml based on the app.yaml and app-livenessProbe.yaml|The kubelet uses readiness probes to know when a container is ready to start accepting traffic|[app-readinessProbe.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-readinessProbe.yaml)|
|app-volumeMounts.yaml|Create app-volumeMounts.yaml. Describe the volumes with livenessProbe, readinessProbe and ports|A volumeMount entails mounting of the declared volume into a container in the same Pod|[app-volumeMounts.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-volumeMounts.yaml)|
|app-cronjob.yaml|Create app-cronjob.yaml based on the app.yaml|A CronJob creates Jobs on a repeating schedule|[app-cronjob.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-cronjob.yaml)|
|app-job.yaml|Create app-job.yaml. Describe the volumes, synchronized containers, volumeMounts|A Job creates one or more Pods and will continue to retry execution of the Pods until a specified number of them successfully terminate|[app-job.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-job.yaml)|
|app-multicontainer.yaml|Create app-multicontainer.yaml. Add three conteiners (nginx, Debian, RedHat)|Manage Multi Container Apps|[app-multicontainer.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-multicontainer.yaml)|
|app-resources.yaml|Create app-resources.yaml for Pod, API v1 as DevOps with livenessProbe, readinessProbe and ports|Organizing resource configurations|[app-resources.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-resources.yaml)|
|app-secret-env.yaml|Create app-secret-env.yaml for Pod, API v1 as DevOps|Using a Secret means that you don't need to include confidential data in your application code|[app-secret-env.yaml](https://github.com/vtomchuk1/kube-prompt/blob/main/yaml/app-secret-env.yaml)|