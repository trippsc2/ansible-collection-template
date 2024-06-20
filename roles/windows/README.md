<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.template.windows
Version: 1.0.1

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
| win_is_vagrant | <p>Whether the machine is to be used as a Vagrant box.</p> | bool | no |  | false |
| win_target_hostname | <p>The hostname to set on the machine.</p><p>This is only used if the machine is a Vagrant box.</p> | str | no |  |  |
| win_set_sshd_manual | <p>Whether to set the OpenSSH service to Manual.</p> | bool | no |  | false |
| win_add_ssh_trusted_ca_cert | <p>Whether to install an SSH trusted CA certificate.</p> | bool | no |  | false |
| win_ssh_trusted_ca_cert_path | <p>The path to the SSH trusted CA certificate.</p><p>This is only used if an SSH trusted CA certificate is to be installed.</p> | str | no |  |  |
| win_ssl_ca_certs | <p>A list of SSL CA certificates to install.</p> | list | no |  |  |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
