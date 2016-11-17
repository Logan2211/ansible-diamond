Diamond Ansible Role
##################################

Ansible role to configure Diamond metrics collection

.. image:: https://travis-ci.org/Logan2211/ansible-diamond.svg?branch=master
    :target: https://travis-ci.org/Logan2211/ansible-diamond

https://github.com/python-diamond/Diamond

Default Variables
=================

.. literalinclude:: defaults/main.yml
   :language: yaml
   :start-after: under the License.

Required Variables
==================

You will need the config_template.py action plugin present in your Ansible plugins path
https://github.com/openstack/openstack-ansible-plugins/blob/master/action/config_template.py

Example Playbook
================

.. code-block:: yaml

    - name: Install diamond
      hosts: all
      user: root
      roles:
        - { role: "diamond" }
