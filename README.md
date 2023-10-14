# Ansible VPN Playbook

![Ansible](https://img.shields.io/badge/ansible-%3E%3D2.9-brightgreen.svg) ![License](https://img.shields.io/github/license/javascriptizer1/ansible-vpn)

This Ansible playbook automates the setup of a VPN (Virtual Private Network) server. You can use it to quickly deploy a VPN server for secure and private network connections.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Configuration](#configuration)
- [License](#license)

## Prerequisites

Before using this playbook, ensure that you have the following prerequisites in place:

- [Ansible](https://www.ansible.com/) installed on your local machine.

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/javascriptizer1/ansible-vpn.git
   ```

2. Navigate to the playbook directory:

   ```bash
   cd ansible-vpn
   ```

3. Edit the **inventory.ini** file to define your target hosts.

4. Customize the **defaults/main.yaml** file to configure your VPN settings.

5. Run the playbook using the following command:

   ```bash
   ansible-playbook -i inventories/inventory.ini -l vpn playbook.yaml --diff -v -vvvv
   ```

Follow the prompts and provide any additional information required during the playbook execution.

Once the playbook completes, your VPN server should be up and running.

## Configuration

You can customize your VPN setup by editing the **defaults/main.yaml** file. Here are some of the parameters you can configure:

- VPN server type (OpenVPN, WireGuard, etc.)
- VPN server port
- DNS server settings
- VPN client settings
- Additional server hardening options

## License

None
