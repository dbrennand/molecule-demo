# molecule-demo

This repository is a demo of how to use [Molecule](https://molecule.readthedocs.io/en/latest/) to test an Ansible playbook.

This repository complements my blog post [Testing Ansible Content with Molecule](https://danielbrennand.com/blog/testing-ansible-content).

The [playbook](playbook.yml) in this repository installs [Nginx](https://www.nginx.com/) on a Debian-based Linux distribution.

## Requirements

- Python >= 3.11
- Docker >= 24.0.5

## Usage

1. Create the Python virtual environment and install the dependencies:

    ```bash
    mkdir -pv ~/.virtualenvs
    python3 -m venv ~/.virtualenvs/molecule-demo
    source ~/.virtualenvs/molecule-demo/bin/activate
    pip install -r requirements.txt
    ```

2. Run the test sequence with Molecule:

    ```bash
    molecule test
    ```
