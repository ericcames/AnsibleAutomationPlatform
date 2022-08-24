# Ansible Automation Platform (AAP)

**Playbook Editing**  
- [Visual Studio Code](https://code.visualstudio.com/ "Code editing Redifined")  
![alt text](https://github.com/ericcames/AnsibleAutomationPlatform/blob/main/images/vscodeext.png "Logo Title Text 1")
- [Are you using VI? Put this in your .vimrc file](https://github.com/ericcames/AnsibleAutomationPlatform/blob/main/files_to_deploy/vimrc "Are you using VI? Put this in your .vimrc file")  
![alt text](https://github.com/ericcames/AnsibleAutomationPlatform/blob/main/images/vimrc.png "Logo Title Text 1")

**Playbook Performance**
- [Windows performance](https://docs.ansible.com/ansible/latest/user_guide/windows_performance.html "Windows performance")  




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

## On server roles documentation

<ul>
  <li>cat /usr/share/doc/rhel-system-roles/network/README.md</li>
</ul>
