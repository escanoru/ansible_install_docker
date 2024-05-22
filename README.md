# Ansible_Install_Jenkins

Ansible helper runbook to install docker from [ansible-role-docker](https://github.com/geerlingguy/ansible-role-docker)

You can adjust the Docker installation options on the `main.yaml` file, to see the full list of parameter passed to the docker role see [Docker defaults/main.yml](https://github.com/geerlingguy/ansible-role-docker/blob/master/defaults/main.yml)

## First time Installation

1. Install the collections and roles from requirements.yaml:

    ```bash
    ansible-galaxy install -r requirements.yaml
    ```

1. Run the playbook on the target node:

    ```bash
    time ansible-playbook main.yaml -u ${USER} -i <node>, -b -K

    ## if run locally:
    time ansible-playbook main.yaml -i "$(hostname -i)", -b -K --connection=local
    ```
