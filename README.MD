#Validate virt_host
Fedora host
Fedora_virt_host
#Validate ipa virt_guest
Ipa virt_guest
Fedora_virt_guest

# Validate freeipa_server
Ipa virt_guest
Freeipa_server

# validate freeipa_demo
Ipa virt_guest
Ipa_demo_data

# IPA inventory script
Fedora_host
ipa_inventory_script

# validate ipa_guests
demo_clients
fedora_virt_guest
ipa_clients


Fedora Laptop:
- (Ansible playbook to build) Fedora VM
- (Ansible playbook to )deploy FreeIPA
- (Ansible playbook to populate) sample data in FreeIPA
- Ansible + IPA inventory script
- Provision some more nodes, join to IPA
  - provision with SSH key in ansible user
  - automember
- Run some playbooks against groups
  - show hbac, sudo
