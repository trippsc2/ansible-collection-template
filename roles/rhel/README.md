<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.template.rhel
Version: 1.0.0

This role seals a RHEL-based machine for use as a template.

## Requirements

| Platform | Versions |
| -------- | -------- |
| EL | <ul><li>8</li><li>9</li></ul> |

## Dependencies

None.

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| rhel_target_hostname | The target hostname. | str | yes |  |  |
| rhel_add_ssh_trusted_ca_cert | Whether to add a SSH trusted CA certificate. | bool | no |  | false |
| rhel_ssh_trusted_ca_cert_path | The path to the SSH trusted CA certificate. Only needed if `rhel_add_ssh_trusted_ca_cert` is `true`. | path | no |  |  |
| rhel_ssl_ca_certificates | List of trusted SSL CA certificates to add. | list | no |  |  |
| rhel_install_cloud_init | Whether to install cloud-init. This is needed for VMware and Nutanix templates. | bool | no |  | false |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
