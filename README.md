# Ansible Role: `Helm`

This role installs [Helm](https://helm.sh) on any supported host.

## Requirements

None

## Role Variables

Variables with default values that can be overridden as part of role defaults (see `defaults/main.yml`):

| Variable | Comments |
| --  | -- |
| helm_version | Sets the version of Helm to install, upgrade or downgrade. Default value is **v3.2.1**
| helm_platform | Corresponds to the OS for which Helm is required. This value is set to **Linux**
| helm_arch | Architecture of the tarball to be downloaded. This value defaults to **amd64**
| helm_url | URL from where helm has to be downloaded. Change this only if required
| helm_path | Path on the OS where Helm binaries are installed. Defaults to /usr/bin/helm


## Dependencies

None.

## Example Playbook

```Yaml
    - hosts: all
      roles:
        - helm
```

## License

BSD

## Author

**Sanjay Singh**
sanjay.kr.singh@gmail.com 
> Written with [StackEdit](https://stackedit.io/).
