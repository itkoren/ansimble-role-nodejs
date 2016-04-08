nodejs
========

Install node js on your mac with n as node package manager and specified node versions
Install npm packages globally

[![Build Status](https://travis-ci.org/itkoren/ansimble-role-nodejs.svg)](https://travis-ci.org/itkoren/ansimble-role-nodejs/)

## Requirements

the same as the ones required by the dependencies

## Role variables
the following are all **optional** and can be applied only as needed:

| Name                  | Description                                      | Default            |
|-----------------------|--------------------------------------------------|--------------------|
| `node_versions`       | The node versions to install                     | `[]`               |
| `node_version`        | The current node version to install              | `[]`               |
| `npm_packages`        | The list of the npm packages to install globally | `[]`               |

## Playbook example
```YAML
---

- hosts: all
  roles:
  - role: itkoren.ansimble-role-nodejs
    node_version:
    - 4.2.4
    node_versions:
    - 0.10.9
    - 0.12.12
    npm_packages:
    - grunt-cli

```
## Dependencies

- `osxc.homebrew`

## License

MIT

## Author

- Itai Koren
