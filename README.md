# How to enable the Pipelines Technology Preview feature in OpenShift Container Platform 3.3

1) As cluster admin exectute the following command:

`oadm policy add-cluster-role-to-group system:build-strategy-jenkinspipeline system:authenticated`

2) You'll also need to [Enable Pipelines in the Web UI] (https://docs.openshift.com/container-platform/3.3/install_config/web_console_customization.html#web-console-enable-tech-preview-feature) and restart your master service:

```systemctl restart atomic-openshift-master``` 

Or for HA installations:

```systemctl restart atomic-openshift-master-api```.


3) Now you can test it with the following example: [Using Jenkins Pipelines with OpenShift] (https://github.com/openshift/origin/tree/master/examples/jenkins/pipeline)
 
