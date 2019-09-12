Role Name
=========

Bootstrap a JIRA Server for use in hmpps ndelius engineering account. Supports legacy version of JIRA (v6.x) 

Requirements
------------

 - boto3
 - botocore

Role Variables
--------------

 - region: AWS Region (default: eu-west-2)
 - cwlogs_log_group: Name of the Cloudwatch Logs Groups for awslogsd target (dfefault: jira-server-cwl)
 - jira_user_home_dir: Home directory for jira user and install files (default: /home/jira)
 - jira_filename: JIRA Server install tarball file name prefix (default: atlassian-jira)
 - jira_version: JIRA Server version (default: 6.4.9)

Dependencies
------------

 - botocore
 - boto3

Example Playbook
----------------

---
- hosts: localhost
  roles:
    - jira-bootstrap

License
-------

MIT

Author Information
------------------

HMPPS Digital Studio
