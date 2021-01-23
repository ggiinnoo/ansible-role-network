Network
=========

This playbook allows you to configure networks in linux

TODO
----

No to do's as of now

Requirements
------------

There are no requirements for this role


Role Variables
--------------

This is an example of a full script install

    networks:
    - name: "eth1"
      type: "Ethernet"
      onboot: "yes"
      bootproto: "dhcp"
      nm_controlled: "no"
      mtu: 9000
      defroute:
      ipv4_failure_fatal:
      ipv6init:
      ipv6_autoconf:
      ipv6_defroute:
      ipv4_failure_fatal:
      uuid:
      hwaddr:
      ipaddr: "10.14.14.6"
      netmask: 255.255.255.0
      prefix:
      network: "10.14.14.0"
      gateway:
      dns1:
      dns2:
      domain:
      ipv6_peerdns:
      ipv6_peerroutes:
      disabled: false


Dependencies
------------

There are no Dependecies for this role

Example Playbook
----------------

    - name: Configure network
      hosts: all
      roles:
        - ggiinnoo.network

License
-------

BSD

Author Information
------------------

    Creator: Gino Jansen
    Website: www.ginojansen.nl
