# cloud-init-config

# This is a collection of configuration files and cloud-init scripts for deploying and configuring various services on cloud instances.

# Repository Structure
The repository is structured as follows:

The configuration-files directory contains all the configuration files required for setting up different services.
The root directory contains cloud-init files that can be used to automate the deployment of services on cloud instances.

# Configuration Files
The configuration-files directory contains subdirectories for each service, and each subdirectory contains the configuration files for that service. Currently, the following services are included:

Elasticsearch
Kibana
Prometheus

Each service directory contains one or more configuration files that can be used to customize the behavior of that service. To use a configuration file, copy it to the appropriate directory on your system and restart the relevant service to apply the changes.

# Cloud-Init Scripts
The root directory contains cloud-init scripts that can be used to automate the deployment of services on cloud instances. Each cloud-init script installs and configures one or more services on an instance. Currently, the following cloud-init scripts are included:

## ELK-setup-cloud-init-script.yml: Installs and configures Elasticsearch and Kibana.
## Prometheus-setup-cloud-init-script.yml: Installs and configures Prometheus.

To use a cloud-init script, copy the contents of the desired file and paste them into the user data section of your cloud instance creation form or API request. For example, if you are using the AWS EC2 console, you can paste the contents of the cloud-init script into the user data field of the instance creation form.
