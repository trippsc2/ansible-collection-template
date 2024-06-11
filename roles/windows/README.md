<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.template.windows
Version: 1.0.0

This role seals a Windows machine for use as a template.

## Requirements

| Platform | Versions |
| -------- | -------- |
| Windows | <ul><li>2019</li><li>2022</li></ul> |

## Dependencies

| Collection |
| ---------- |
| ansible.windows |
| community.windows |

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| win_is_vagrant | Whether the machine is to be used as a Vagrant box. | bool | no |  | false |
| win_target_hostname | The hostname to set on the machine. This is only used if the machine is a Vagrant box. | str | no |  |  |
| win_set_sshd_manual | Whether to set the OpenSSH service to Manual. | bool | no |  | false |
| win_add_ssh_trusted_ca_cert | Whether to install an SSH trusted CA certificate. | bool | no |  | false |
| win_ssh_trusted_ca_cert_path | The path to the SSH trusted CA certificate. This is only used if an SSH trusted CA certificate is to be installed. | str | no |  |  |
| win_ssl_ca_certs | A list of SSL CA certificates to install. | list | no |  |  |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
