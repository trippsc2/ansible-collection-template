<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.template.debian
Version: 1.0.0

This role seals a Debian machine for use as a template.

## Requirements

| Platform | Versions |
| -------- | -------- |
| Debian | <ul><li>bullseye</li><li>bookworm</li></ul> |

## Dependencies

None.

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| debian_target_hostname | The target hostname. | str | yes |  |  |
| debian_add_ssh_trusted_ca_cert | Whether to add a SSH trusted CA certificate. | bool | no |  | false |
| debian_ssh_trusted_ca_cert_path | The path to the SSH trusted CA certificate. Only needed if `debian_add_ssh_trusted_ca_cert` is `true`. | path | no |  |  |
| debian_ssl_ca_certificates | List of trusted SSL CA certificates to add. | list | no |  |  |
| debian_install_cloud_init | Whether to install cloud-init. This is needed for VMware and Nutanix templates. | bool | no |  | false |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
