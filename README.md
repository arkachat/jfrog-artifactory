


This playbook installs artifactory  at /opt location .


###Playbook variables

We have defined below mentioned variables for our playbook.


```
artifactory_version: artifactory-oss-6.8.4
artifactory_dir: /opt/{{ artifactory_version }}
artifactory_zip_file: artifactory-oss-6.8.4.zip
artifactory_zip_url: http://dl.bintray.com/content/jfrog/artifactory/jfrog-"{{ artifactory_zip_file }}"

```

####Current Required functionalities.
- Use of database  for  artifactory
- Allow repository creation and configuration.