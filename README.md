mirror-registry
===============
Deploys a simple v2 based container registry, with authentication and https support.

Implementation based from Red Hat documentation on setting up a Mirror Registry for OCP 4.x:\
https://access.redhat.com/documentation/en-us/openshift_container_platform/4.4/html/installing/installation-configuration#installing-restricted-networks-preparations


Requirements
------------
* Create an inventory file for your deployment
* Override the following variables:
  * `mirror_registry_cert:` - The contents of the SSL certificate file for the mirror registry
  * `mirror_registry_key:` - The contents of the SSL private key file for the mirror registry

Usage
-----
* Deploy the mirror registry on an already configured VM/instance:
```
ansible-playbook deploy_mirror_registry.yml
```

TODO
----
* Greater customisation for the deployed mirror registry
