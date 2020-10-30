## mailcatcher

[![Build Status](https://travis-ci.org/Oefenweb/ansible-mailcatcher.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-mailcatcher)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-mailcatcher-blue.svg)](https://galaxy.ansible.com/Oefenweb/mailcatcher/)

Set up (the latest version of) [MailCatcher](http://mailcatcher.me/) in Ubuntu systems.

#### Requirements

* `ruby2.*` (will be installed)
* `ruby2.*-dev` (will be installed)
* `libsqlite3-dev` (will be installed)
* `build-essential` (will be installed)

#### Variables

* `mailcatcher_version`: [default: `latest`]: MailCatcher version to install (e.g. `latest`, `0.6.4`)

* `mailcatcher_user` [default: `mailcatcher`]: The user that will run the `mailcatcher` daemon
* `mailcatcher_group` [default: `mailcatcher`]: The primary group of the `mailcatcher` user
* `mailcatcher_groups` [default: `[]`]: The secondary groups of the `mailcatcher` user

* `mailcatcher_options: {}`]: Options to pass to the `mailcatcher` daemon (e.g. `{ip: 0.0.0.0}`)

## Dependencies

None

## Recommended

None

#### Example (without any options)

```yaml
---
- hosts: all
  roles:
    - mailcatcher
```

#### Example (with daemon options)

```yaml
---
- hosts: all
  roles:
    - mailcatcher
  vars:
    mailcatcher_options:
      ip: 0.0.0.0
```

#### License

MIT

#### Author Information

Mischa ter Smitten (based on work of [yauh](https://github.com/yauh) and [vranac](https://github.com/vranac))

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-mailcatcher/issues)!
