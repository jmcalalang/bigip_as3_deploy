# This solution will deploy an example AS3 application with the v2 ansible module from F5.

## Install AS3 on the BIG-IP
 - https://clouddocs.f5.com/products/extensions/f5-appsvcs-extension/latest/userguide/installation.html?highlight=install

## Install Ansible
 - mac (brew install ansible)

## Install Ansible Galaxy collection
 - https://clouddocs.f5.com/products/orchestration/ansible/devel/f5_bigip/install_f5_bigip.html
   - mac ( ansible-galaxy collection install f5networks.f5_bigip )

### The task is located in ```f5_modules-as3``` the playbook is called ```app_new.yml```

### Run the Ansible playbook from the root of the folder.

```ansible-playbook -i inventory/hosts f5_modules-as3/app_new.yml```
