## mailcatcher

[![Build Status](https://travis-ci.org/Oefenweb/ansible-mailcatcher.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-mailcatcher) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-mailcatcher-blue.svg)](https://galaxy.ansible.com/Oefenweb/mailcatcher/)

Set up (the latest version of) [MailCatcher](http://mailcatcher.me/) in Debian-like systems.

#### Requirements

* `ruby` (will be installed)
* `ruby-dev` (will be installed)
* `build-essential` (will be installed)

#### Variables

* `mailcatcher_version`: [default: `latest`]: MailCatcher version to install (e.g. `latest`, `1.9.2`)

## Dependencies

None

## Recommended

None

#### Example

```yaml
---
- hosts: all
  roles:
    - mailcatcher
```

#### License

MIT

#### Author Information

Mischa ter Smitten (based on work of [yauh](https://github.com/yauh) and [vranac](https://github.com/vranac))

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-mailcatcher/issues)!
