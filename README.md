# helm-chart-portal
k8s package manager
Create new helm repo:$ helm create repoName

Check actual value of placeholders:$ helm template helmChartName(helm-chart-portal)

Check compilation errors:$ helm lint helmChartName(helm-chart-portal) 

Check deployment/installation errors:$ helm install releaseName(anyString) --debug --dry-run helmChartName(helm-chart-portal) 

Install/Deploy chart :$ helm install releaseName(anyString) helmChartName(helm-chart-portal)

Check installed chart deployed successfully or not:$ helm list -a

Redeploy/upgrade charts: increase version number ::$ helm upgrade releaseName(anyString) helmChartName(helm-chart-portal)

Downgrade/rollback: $ helm rollback releaseName(anyString) versionNo(like 1)

Clean up/delete helm: $ helm delete releaseName

**Revision number**: it is a release number
For multi service application deployment like this portal having multiple docker services use subcharts concept with dependency tag & create chart for every service in charts folder.


