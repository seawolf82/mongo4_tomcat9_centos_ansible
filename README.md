# mongo4_tomcat9_centos7

This script install mongodb CE version 4.4 and tomcat 9 (9.0.68) on Red Hat Based Distributions


Tested with openjdk17 on Almalinux8-9 RockyLinux8-9
Tested with openjdk18 on Centos7

Tested on:

- Almalinux 8
- Almalinux 9
- RockyLinux 8
- RockyLinux 9
- Centos 7

Tested on:

- 2.9 Ansible version


To install mongo4 and tomcat9 on Red Hat Based Distributions run:

ansible-playbook -i hosts site.yaml

To uninstall mongo4 and tomcat9 on Red Hat Based Distributions run

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
ntp
mongodb
tomcat


For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
