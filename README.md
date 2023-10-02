Ansible Role: ELK Stack Download

This Ansible role simplifies the process of downloading and setting up the ELK (Elasticsearch, Logstash, and Kibana) stack on your target hosts. The ELK stack is a powerful tool for collecting, indexing, and visualizing log and event data.
Requirements

Before using this role, ensure you have the following prerequisites:

    Ansible is installed on your control machine.
    Your target hosts have internet access to download the required ELK stack components.

Role Variables

This role does not have specific variables to configure. It uses predefined settings for downloading the ELK stack components. However, you can customize the version or other settings in your Ansible playbook using the vars section.
Dependencies

This role does not have any dependencies on other Ansible roles.
Example Playbook

Here's an example playbook that demonstrates how to use this role:

```
---
- name: Configure DNS servers
  hosts: all
  become: yes
  roles:
    - ELK_install
```

License

This Ansible role is licensed under the MIT License. Feel free to modify and distribute it as needed for your projects.
