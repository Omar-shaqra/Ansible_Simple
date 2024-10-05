
# Ansible_Simple

This repository provides a simple and straightforward example of using **Ansible** for configuration management and automation. The playbooks and roles in this project demonstrate basic usage of Ansible for managing server configurations and automating routine tasks.

## Table of Contents
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
  - [Running Playbooks](#running-playbooks)
  - [Example Playbook](#example-playbook)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Overview

Ansible is an open-source automation tool used for IT tasks such as configuring servers, deploying applications, and orchestrating IT workflows. This repository includes example Ansible playbooks and roles to help you get started with basic Ansible automation.

## Prerequisites

Before using the content in this repository, ensure you have the following installed:
- **Ansible**: Install it on your control node (local machine). You can follow the official [Ansible installation guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).
- **SSH Access**: You need SSH access to the remote servers you want to manage.

## Installation

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Omar-shaqra/Ansible_Simple.git
   cd Ansible_Simple
   ```

2. Ensure Ansible is installed on your system:
   ```bash
   sudo apt update
   sudo apt install ansible -y
   ```

3. Set up your inventory file to point to the target hosts you want to manage with Ansible.

## Usage

### Running Playbooks

You can run Ansible playbooks from this repository using the following command:

```bash
ansible-playbook -i inventory playbook.yml
```

- `-i inventory`: Specifies the inventory file.
- `playbook.yml`: Replace with the playbook you want to execute.

### Example Playbook

Below is a basic example of how to use one of the playbooks from this repository:

```bash
ansible-playbook -i inventory/setup-server.yml
```

This command will apply the `setup-server.yml` playbook to the hosts defined in the `inventory` file.

## Project Structure

The repository structure is as follows:

```
Ansible_Simple/
├── inventory          # Inventory file with target hosts
├── playbook.yml       # Sample playbook
├── roles/             # Ansible roles
│   ├── role1/         # Example role directory
│   └── role2/         # Another example role directory
├── group_vars/        # Group-specific variables
├── host_vars/         # Host-specific variables
└── README.md          # This README file
```

- **inventory**: The inventory file lists the hosts that Ansible will target.
- **playbook.yml**: The main playbook file that Ansible executes.
- **roles/**: Contains reusable Ansible roles for modular playbooks.

## Contributing

Contributions to this repository are welcome! If you have any improvements or additional features you'd like to add, feel free to open a pull request or submit an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
