# vnios-autoscale-ansible
Autoscale vnios on Openstack using Ansible

Autoscaling vNIOS on Openstack solution using ansible, is a combination of shell script and ansible playbook.
While the shell script uses a combination of DNS QPS and CHR values to determine if there is a need to spin a new member, ansible playbook does all the heavy lifting. Ansible playbook deploys the new member initializes, it adds it to the grid and makes it part of a nameserver group and anycast configuration.

Requirememts :
Ubuntu 16.04 LTS machine with root access and a Openstack with sufficient resources to host Infoblox Grid( Grid master and 3 Members)
