<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.template.ubuntu
Version: 1.0.0

This role seals an Ubuntu machine for use as a template.

## Requirements

| Platform | Versions |
| -------- | -------- |
| Ubuntu | <ul><li>focal</li><li>jammy</li><li>noble</li></ul> |

## Dependencies

None.

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| ubuntu_target_hostname | The target hostname. | str | yes |  |  |
| ubuntu_add_ssh_trusted_ca_cert | Whether to add a SSH trusted CA certificate. | bool | no |  | false |
| ubuntu_ssh_trusted_ca_cert_path | The path to the SSH trusted CA certificate. Only needed if `ubuntu_add_ssh_trusted_ca_cert` is `true`. | path | no |  |  |
| ubuntu_ssl_ca_certificates | List of trusted SSL CA certificates to add. | list | no |  |  |
| ubuntu_install_cloud_init | Whether to install cloud-init. This is needed for VMware and Nutanix templates. | bool | no |  | false |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
