# AnsibleAutomationPlatform

## Ansible facts

<ul>
  <li>ansible all -m setup</li>
</ul>

## Ansible facts for storage

<ul>
  <li>ansible all -m setup -a 'filter=ansible_devices'</li>
  <li>ansible all -m setup -a 'filter=ansible_device_links'</li>
  <li>ansible all -m setup -a 'filter=ansible_mounts'</li>
  <li>ansible all -a lsblk</li>
</ul>

## Ansible facts for network

<ul>
  <li>ansible webservers -m setup -a 'gather_subset=network filter=ansible_interfaces'</li>
  <li>ansible webservers -m setup -a 'gather_subset=network filter=ansible_ens4'</li>
</ul>
