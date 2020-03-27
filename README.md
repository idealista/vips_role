![Logo](https://raw.githubusercontent.com/idealista/vips_role/master/logo.gif)

[![Build Status](https://travis-ci.org/idealista/vips_role.svg?branch=master)](https://travis-ci.org/idealista/vips_role)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-idealista.vips__role-B62682.svg)](https://galaxy.ansible.com/idealista/vips_role)
[![Docker Hub pulls](https://img.shields.io/docker/pulls/idealista/vips.svg)](https://hub.docker.com/r/idealista/vips/)

# Vips Ansible role

This Ansible role installs libvips image processing library in a Debian environment.

- [Getting Started](#getting-started)
	- [Prerequisities](#prerequisities)
	- [Installing](#installing)
- [Usage](#usage)
- [Testing](#testing)
- [Built With](#built-with)
- [Versioning](#versioning)
- [Authors](#authors)
- [License](#license)
- [Contributing](#contributing)

## Getting Started

These instructions will get you a copy of the role for your Ansible Playbook. Once launched, it will install [libvips](https://libvips.github.io/libvips/) libraries.

### Prerequisities

Ansible 2.9.6.0 version installed.
Inventory destination should be a Debian environment.

For testing purposes, [Molecule](https://molecule.readthedocs.io/) with [Docker](https://www.docker.com/).

### Installing

Create or add to your roles dependency file (e.g requirements.yml):

```
- src: idealista.vips_role
  version: 2.0.0
  name: vips
```

Install the role with ansible-galaxy command:

```
ansible-galaxy install -p roles -r requirements.yml -f
```

Use in a playbook:

```
- hosts: someserver
  roles:
    - role: vips
```

## Usage

Look to the [defaults](defaults/main.yml) properties file to see the possible configuration properties.

[orc](https://github.com/GStreamer/orc) version supported >= 0.4.20

## Testing

```sh
$ pip install pipenv
$ pipenv sync
```

## Built With

![Ansible](https://img.shields.io/badge/ansible-2.9.6.0-green.svg)
![Molecule](https://img.shields.io/badge/molecule-2.22.0-green.svg)
![Goss](https://img.shields.io/badge/goss-0.3.7-green.svg)

## Versioning

For the versions available, see the [tags on this repository](https://github.com/idealista/vips_role/tags).

Additionaly you can see what change in each version in the [CHANGELOG.md](CHANGELOG.md) file.

## Authors

* **Idealista** - *Work with* - [idealista](https://github.com/idealista)

See also the list of [contributors](https://github.com/idealista/vips_role/contributors) who participated in this project.

## License

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

This project is licensed under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license - see the [LICENSE](LICENSE) file for details.

## Contributing

Please read [CONTRIBUTING.md](.github/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
