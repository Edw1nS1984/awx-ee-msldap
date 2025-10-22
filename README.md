# awx-ee-msldap

This repository provides an AWX Execution Environment (EE) image tailored for working with Microsoft Active Directory using LDAP via Ansible. It is designed to simplify automation workflows with AWX when managing Active Directory resources using the [`microsoft.ad.ldap`](https://galaxy.ansible.com/microsoft/ad.ldap) Ansible collection.

## What does this project do?

- **AWX EE Base Image**: Extends the standard AWX EE image with additional dependencies required for Microsoft AD LDAP automation.
- **Pre-installed Ansible Collection**: Includes the `microsoft.ad.ldap` collection, enabling modules and plugins for managing Microsoft Active Directory objects using LDAP.
- **Dependency Management**: Ensures all necessary Python and system packages required by the collection are present in the environment, reducing setup friction.

## Key Features

- Out-of-the-box support for Microsoft AD LDAP tasks with Ansible.
- Ready for use in AWX and Automation Controller.
- Easy to extend with additional Ansible collections or Python requirements.

## Dependencies

This execution environment includes:

- [`microsoft.ad.ldap`](https://galaxy.ansible.com/microsoft/ad.ldap) Ansible collection.
- All Python and system dependencies required by the collection.
- Base packages for AWX EE operation.

## Usage

1. Build or pull the image defined in this repository.
2. Use it as your custom Execution Environment in AWX or Automation Controller.
3. Write Ansible playbooks using modules from the `microsoft.ad.ldap` collection to automate LDAP operations against Microsoft AD.

## Customization

You can customize the included dependencies by editing the `requirements.yml` (for Ansible collections) and `requirements.txt` (for Python packages) provided in this repository. Rebuild the image after changes.

## License

MIT License (or specify your license here).

## Reference

- [Ansible Collection: microsoft.ad.ldap](https://galaxy.ansible.com/microsoft/ad.ldap)
- [AWX EE Documentation](https://github.com/ansible/awx-ee)