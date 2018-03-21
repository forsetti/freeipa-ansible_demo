= demo.xml =
== Validate virt_host ==
  - Fedora host
  - Fedora_virt_host

== Create ansible control VM ==
  - Pack ansible content into cidata
  - Ansible control virt_guest
  - Ansible control install ansible packages
  - Execute ansible playbook on site.yml

= site.yml =
== Validate virt_host ==
  - Fedora host
  - Fedora_virt_host
== Validate ipa virt_guest ==
  - Ipa virt_guest
  - Fedora_virt_guest

== Validate freeipa_server ==
  - Ipa virt_guest
  - Freeipa_server

== validate freeipa_demo ==
  - Ipa virt_guest
  - Ipa_demo_data
     - users
     - groups
     - host-groups
     - sudo
     - hbac

== IPA inventory script ==
  - Fedora_host
  - ipa_inventory_script

== validate ipa_guests ==
  - demo_clients
  - fedora_virt_guest
  - ipa_clients
