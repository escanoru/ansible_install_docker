# Ansible_Install_Jenkins

Ansible helper runbook to install docker from well known roles

## First time Installation

1. Install the collections and roles from requirements.yaml:

    ```bash
    ansible-galaxy install -r requirements.yaml
    ```

1. Run the playbook on the target node:

    ```bash
    time ansible-playbook main.yaml -u ${USER] -i <node>, -b -K
    ```
