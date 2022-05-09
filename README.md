# AnsibleAutomationPlatform

## Ansible facts for storage

<ul>
  <li>ansible webservers -m setup</li>
  <li>ansible webservers -m setup -a 'filter=ansible_devices'</li>
  <li>ansible webservers -m setup -a 'filter=ansible_device_links'</li>
  <li>ansible webservers -m setup -a 'filter=ansible_mounts'</li>
  <li>ansible all -a lsblk</li>
</ul>
