# nephelaiio.elastic-repo

[![Build Status](https://github.com/nephelaiio/ansible-role-elastic-repo/actions/workflows/molecule.yml/badge.svg)](https://github.com/nephelaiio/ansible-role-elastic-repo/actions/workflows/molecule.yml)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-nephelaiio.elastic-repo.vim-blue.svg)](https://galaxy.ansible.com/nephelaiio/elastic-repo/)

An [ansible role](https://galaxy.ansible.com/nephelaiio/elastic_repo) to install and configure Elasticsearch's repositories

## Role Variables

The most common user overridable parameters for the role are

| required | variable | description | default |
| --- | --- | --- | --- |
| no | elasticsearch_repo_oss | whether to install the oss version of the repository | yes |
| no | elasticsearch_repo_state | the state of the repository | present |

Please refer to the [defaults file](/defaults/main.yml) for an up to date list of input parameters.

## Example Playbook

```
- hosts: servers
  roles:
     - role: nephelaiio.elastic_repo
```

## Testing

Please make sure your environment has [docker](https://www.docker.com) installed in order to run role validation tests. Additional python dependencies are listed in the [requirements file](https://github.com/nephelaiio/ansible-role-requirements/blob/master/requirements.txt)

Role is tested against the following distributions (docker images):
  * Ubuntu Focal
  * Ubuntu Bionic
  * Ubuntu Xenial
  * CentOS 7
  * Debian Buster

You can test the role directly from sources using command ` molecule test `

## License

This project is licensed under the terms of the [MIT License](/LICENSE)
