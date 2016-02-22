# Ansible Role: Zookeeper

An Ansible role that installs Zookeeper on supported Ubuntu LTS releases.

## Requirements

No special pre-requisites.

Role Variables
--------------

    - name: apt_cache_valid_time
      description: update apt cache if it is older than this
      default: None

    - name: zookeeper_enabled
      description: whether zookeeper should be enabled by default
      default: true

    - name: zookeeper_state
      description: zookeeper service state after running this role
      default: started

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: traveloka.zookeeper
	  apt_cache_valid_time: 3600

License
-------

Apache

Author Information
------------------

Author: Michel Alexandre Salim <michel@traveloka.com>
Copyright (C) Traveloka 2016
https://github.com/traveloka

