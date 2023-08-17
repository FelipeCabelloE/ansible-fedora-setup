# ansible-fedora-setup

Installs and configures most of the software I use on Fedora Workstation following a minimal install.

## Usage

### Pre-installation
1. Install git: `dnf install git`
2. Install Ansible: `dnf install ansible`
    - (Optional) I prefer to install Ansible with `pip` inside a `virtualenv`:
        ```bash
        dnf install python-virtualenv
        virtualenv ansible-env
        source ansible-env/bin/activate
        pip install ansible selinux
        ```
3. Clone this repository: `git clone https://github.com/FelipeCabelloE/ansible-fedora-setup`

### Running the Playbook
Change into the playbook directory and run `ansible-playbook`:
```bash
cd ansible-fedora-setup/
ansible-playbook -K playbook.yml
```


##TODO
I have to update to my actual setup in preparation for fedora 38

Some of the changes that i have to take in consideration is the usage of pycharm, speedup of firefox using env variable, and the integration of starship with (maybe?) fish

see installation instructions for more ideas on necesary changes.

Maybe I could setup juppyter 