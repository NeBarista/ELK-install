Ansible Role: Elastic Stack Docker Download

This Ansible role is designed to simplify the process of downloading and setting up the Elastic Stack (Elasticsearch, Kibana, Logstash, Beats) using Docker containers on your target hosts. The Elastic Stack is a powerful tool for collecting, indexing, and visualizing data.
Requirements

Before using this role, ensure you have the following prerequisites:

    Ansible is installed on your control machine.
    Docker is installed on your target hosts.
    Your target hosts have internet access to pull Docker images from the Elastic Docker registry.

Role Variables

This role does not have specific variables to configure. It uses predefined Docker image names for the Elastic Stack components. However, you can customize the version or other settings in the Ansible playbook using the vars section.
Dependencies

This role doesn't have any dependencies on other Ansible roles.
Example Playbook

Here's an example playbook that demonstrates how to use this role:

yaml

- name: Download Elastic Stack Docker Images
  hosts: your_target_hosts
  become: yes  # If privilege escalation is required (sudo)
  roles:
    - name: Download Elastic Stack Docker Images
      role: elastic-stack-docker-download

In this example, replace your_target_hosts with the appropriate host group or host(s) where you want to download the Elastic Stack Docker images. You can further customize this playbook by specifying the version of Elastic Stack components or other configuration settings.
License

This Ansible role is licensed under the MIT License. Feel free to modify and distribute it as needed for your projects.
