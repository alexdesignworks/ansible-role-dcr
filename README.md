# Ansible Role DCR (Drupal Code Review)

An Ansible role that installs [DCR](https://github.com/alexdesignworks/dcr).

## Role Variables

Available variables are listed below, along with default values:

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

## Dependencies

`geerlingguy.composer`

## License

MIT
