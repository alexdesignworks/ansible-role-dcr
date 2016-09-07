# Ansible Role DCR (Drupal Code Review)

An Ansible role that installs [DCR](https://github.com/alexdesignworks/dcr).

## Role Variables

Available variables are listed below, along with default values:

DCR version.
```
dcr_version: "~0.1"
```

Directory to install DCR into.
```
dcr_install_dir: "/var/www"
```

Initialise DCR after install.
```
dcr_init: yes
```

Initialise DCR in directory.
```
dcr_init_dir: "{{ dcr_install_dir }}"
```

List of target files and directories to scan.
```
dcr_targets:
  - sites/all/modules/custom
  - sites/all/themes/custom
```

List of extensions to scan.
```
dcr_extensions:
  - module
  - install
  - profile
  - php
  - theme
  - inc
  - test
  - js
```

Success message.
```
dcr_success_message: "All good! You're awesome!"
```

Fail message.
```
dcr_fail_message: "Please fix errors above and re-run dcr"
```


## Dependencies

`geerlingguy.composer`

## License

MIT
