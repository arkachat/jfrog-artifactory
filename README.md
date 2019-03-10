bbaassssiiee.artifactory
=========

Install Artifactory, the Maven repository manager by JFrog.

Requirements
------------

This role was built for RedHat systems like RHEL 6, Centos 6. It needs Java, and PostgreSQL or MySQL.

Role Variables
--------------
artifactory_database can hold either 'mysql' or 'postgresql', you should provide the database yourself now,
it is no longer a transitive dependency.

artifactory_password is defined in defaults/main/yml, override it in group_vars.

artifactory_version is defined in vars/main.yml
Set JAVA_OPTIONS in templates/etc-opt-jfrog-artifactory-default.j2

Dependencies
------------
ansible-galaxy install -p roles pcextreme.mariadb
ansible-galaxy install -p roles geerlingguy.java

