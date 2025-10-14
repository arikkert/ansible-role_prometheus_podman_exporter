prometheus_podman_exporter
==========================

Install and run prometheus-podman-exporter and open firewall for this service if needed

Requirements
------------

For RedHat OS family
EPEL repo (will be installed if not found)
Tested on Almalinux 9

Role Variables
--------------

*prometheus_ip* (optional), the ip of the prometheus host. \
Only used in RedHat os family. \
If firewall is already running. \
If defined, the firewall is configured to allow scraping from only the *prometheus_ip*. \
If not defined, the firewall is configured to allow access to the exporter from all hosts

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles
         - role: arikkert.prometheus_podman_exporter
           prometheus_ip: 1.2.3.4

License
-------

BSD

Author Information
------------------

    ARK-ICT
    Andre Rikkert de Koe - ICT
