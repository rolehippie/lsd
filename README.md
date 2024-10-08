# lsd

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/lsd)
[![General Workflow](https://github.com/rolehippie/lsd/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/lsd/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/lsd/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/lsd/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/lsd/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/lsd/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/lsd)](https://github.com/rolehippie/lsd/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.lsd-blue)](https://galaxy.ansible.com/rolehippie/lsd)

Ansible role to install lsd the ls replacement.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [lsd_arch](#lsd_arch)
  - [lsd_download](#lsd_download)
  - [lsd_version](#lsd_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### lsd_arch

Architecture of the package to install

#### Default value

```YAML
lsd_arch: '{{ ansible_architecture }}-unknown-linux-musl'
```

### lsd_download

URL to the archive of the release to install

#### Default value

```YAML
lsd_download: https://github.com/lsd-rs/lsd/releases/download/v{{ lsd_version }}/lsd-v{{
  lsd_version }}-{{ lsd_arch }}.tar.gz
```

### lsd_version

Version of the release to install

#### Default value

```YAML
lsd_version: 1.1.5
```

## Discovered Tags

**_lsd_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
