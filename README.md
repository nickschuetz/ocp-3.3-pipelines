# How to enable the Pipelines Technology Preview feature in OpenShift Container Platform 3.3

1. As cluster admin exectute the following command:

`oadm policy add-cluster-role-to-group system:build-strategy-jenkinspipeline system:authenticated`
...
2. [Enable pipleines in the Web UI] (https://docs.openshift.com/container-platform/3.3/install_config/web_console_customization.html#web-console-enable-tech-preview-feature)
