### Role for installation of Container Runtime Interface (cri-o) for Ubuntu/CentOS

This role based on repos and information from [Kubernetes Container runtimes](https://kubernetes.io/docs/setup/production-environment/container-runtimes/) in addition it installs crictl.

#### Variables
| Variable | Default |
| ------ | ------ |
| crio_version | 1.20 |
| crio_ctl_version | v1.21.0 |

#### Example Playbook
```
---
- hosts: localhost
  remote_user: user
  roles:
    - { role: 'cri-o', tags: "cri-o"}
```

#### License
GNU General Public License v3.0