# Debian Security

1. [Overview](#overview)
2. [Role Variables](#role-variables)
3. [Example Playbook](#example-playbook)
4. [Configuration](#configuration)
5. [Known Issues](#known-issues)
6. [Development](#development)
7. [License](#license)
8. [Author Information](#author-information)

## Overview

A role that provide some security tools for Debian.

## Role Variables

* **deb_sec__required_packages** : List of required packages [default : `debsecan`]
* **deb_sec__deploy_state** : The desired state this role should achieve. [default : `present`].

## Example Playbook

* Default behaviour :

``` yaml
- hosts: my.debian.host
  roles:
    - role: ipr-cnrs.debian_security
```

## Configuration

This role will :
* Install some security tools (eg. Debsecan,…).

## Development

This source code comes from our [Gogs instance][debian_security source] and the [Github repo][debian_security github] exist just to be able to send the role to Ansible Galaxy…

But feel free to send issue/PR anywhere :)

Thanks to this [hook][gogs to github hook], Github automatically got updates from our [Gogs instance][debian_security source] :)

## License

[WTFPL][wtfpl website]

## Author Information

Jérémy Gardais
* Source : [on IPR's Gogs][debian_security source]
* [IPR][ipr website] (Institut de Physique de Rennes)

[gogs to github hook]: https://stackoverflow.com/a/21998477
[debian_security source]: https://git.ipr.univ-rennes1.fr/cellinfo/ansible.debian_security
[debian_security github]: https://github.com/ipr-cnrs.debian_security
[wtfpl website]: http://www.wtfpl.net/about/
[ipr website]: https://ipr.univ-rennes1.fr/