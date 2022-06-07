prometheus-node-exporter
=========

Add default node exporter to debian ubuntu server

Requirements
------------
ansible 2.9 


Role Variables
--------------
You can set a default version by default the last one 
url  **https://github.com/prometheus/node_exporter/releases/download/**
--
**node_version**  1.3.1 ( last version in 2021)

**node_prometheus** ip of your prometheus node scraper
Dependencies
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
