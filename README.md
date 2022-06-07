prometheus-node-exporter
=========

Add default node exporter to debian ubuntu server

Requirements
------------
ansible 2.9 

by default the role have the github url for node exporter 
https://github.com/prometheus/node_exporter/releases/download/

Role Variables
--------------

| **node_version**    | 1.3.1                                                          |
|-----------------|----------------------------------------------------------------    |
| **node_prometheus** | ip for your distante prometheus server                         |

------------
 actually no dependencies for this roles

Example Playbook
----------------

     ansible-playbook -i  inventory/hosts  -u user  prometheus-config.yml    -e "node_version=1.3.1 node_prometheus=127.0.0.1" --limit=server
---
    - hosts: servers
      roles:
         - prometheus-node-exporter

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
