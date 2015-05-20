Ansible Role - mtchavez.envconsul
=========
[![Latest Version](http://img.shields.io/github/release/mtchavez/ansible-envconsul.svg?style=flat-square)](https://github.com/mtchavez/ansible-envconsul/releases)
[![Build Status](https://travis-ci.org/mtchavez/ansible-envconsul.svg?branch=master)](https://travis-ci.org/mtchavez/ansible-envconsul)

[Envconsul](https://github.com/hashicorp/envconsul) provides a convenient way to populate values from [Consul](https://github.com/hashicorp/consul) into an child process environment using the envconsul daemon.

Requirements
------------

No requirements needed to install envconsul

Role Variables
--------------

Useful variables to configure such as the version and arch or even where it is downloaded.

```yaml
envconsul_ver: "0.5.0"
envconsul_arch: "linux_amd64"
envconsul_dl_dir: "/tmp"
envconsul_bin_path: "/usr/local/bin"
```

Dependencies
------------

No external dependencies

Example Playbook
----------------

Install envconsul at a specific version

    - hosts: servers
      roles:
         - { role: mtchavez.envconsul, envconsul_ver: "5.0.0" }

License
-------

MIT

Author Information
------------------

mtchavez - 2015
