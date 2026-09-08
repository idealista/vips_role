# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/) and [Keep a changelog](https://github.com/olivierlacan/keep-a-changelog).

## [Unreleased](https://github.com/idealista/vips_role/tree/develop)

## [2.0.1](https://github.com/idealista/vips_role/tree/2.0.1)
### Fixed
- *[#23](https://github.com/idealista/vips_role/issues/23) Correct the Goss badge, restore the command to run the tests, and document the 2.0.0 move of `libexif-dev` and `libmagick-dev` to `vips_optional_dependencies`* @danieljesus
### Removed
- *[#23](https://github.com/idealista/vips_role/issues/23) Drop the orphaned `test-requirements.txt`, superseded by the Pipfile* @danieljesus

## [2.0.0](https://github.com/idealista/vips_role/tree/2.0.0)
Major release: `vips_force_reinstall` is gone, `vips_version` now defaults to 8.9.1, `min_ansible_version` is 2.9.6.0, and consumers that relied on `libexif-dev` or `libmagick-dev` being pulled in by `vips_required_libs` must now ask for them through `vips_optional_dependencies`.
### Added
- *[#19](https://github.com/idealista/vips_role/pull/19) (2024-01-17)- Add ".gitattributes" file for linguist detection.* @ygomezsaiz
### Changed
- *(https://github.com/idealista/vips_role/pull/12) Allow to override optional dependencies* @dortegau
- *(https://github.com/idealista/vips_role/pull/10) Upgrade Ansible, Molecule and Goss* @dortegau
### Removed
- *(https://github.com/idealista/vips_role/pull/10) Drop `vips_force_reinstall`, and move `libexif-dev` and `libmagick-dev` out of `vips_required_libs` into the new `vips_optional_dependencies`* @dortegau
### Fixed
- *[#20](https://github.com/idealista/vips_role/issues/20) Point the molecule containers at archive.debian.org, all three tested Debian suites are EOL* @danieljesus
- *(https://github.com/idealista/vips_role/pull/8) Update ansible loop and test syntax* @tgjohnst

## [1.0.1](https://github.com/idealista/vips_role/tree/1.0.1)
### Changed
- *(https://github.com/idealista/vips_role/pull/4) Rename role to vips_role* @jnogol
- *(https://github.com/idealista/vips_role/pull/4) Use of pipenv and Debian Stretch base image for tests* @jnogol
### Fixed
- *(https://github.com/idealista/vips_role/pull/3) Update libvips source URL* @chadwilken
- *(https://github.com/idealista/vips_role/pull/6) Fix Travis deploy installing ca-certificates package* @jnogol

## [1.0.0](https://github.com/idealista/vips_role/tree/1.0.0)
### Added
- *First release* @jmonterrubio
