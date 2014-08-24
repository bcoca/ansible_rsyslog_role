Role Name
=========

Installs and configures rsyslog directly from rsyslog.com repos

Requirements
------------

None

Role Variables
--------------

Selects the version of the repo, which determines version installed (check rsyslog.com for valid values):

    rsyslog_repo_version: v7-stable

You can set ElasticSearch with these:

    # ES defaults
    elasticsearch_server: localhost
    elasticsearch_port: 9200
    elasticsearch_rsyslog_queue_size: 5000
    elasticsearch_rsyslog_batch_size: 300

Dependencies
------------

None


Example Playbook
----------------



    - hosts: all
      roles:
         - { role: rsyslog }

License
-------

GPLv2
