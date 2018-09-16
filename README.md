# Ansible Role: ocstore_rollback

Rollback ocStore on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    ocstore_hostname: "localhost"
    
    ocstore_www_root: "/var/www/{{ ocstore_hostname }}"
    
    ocstore_releases_dir: "releases"
    ocstore_current_dir: "current"
    
    ocstore_remove_rolled_back: yes
    
    ocstore_rollback_to_release: ""

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - Akman.ocstore_rollback

*Inside `vars/main.yml`*:

    ocstore_hostname: "localhost"
    
    ocstore_www_root: "/var/www/{{ ocstore_hostname }}"
    
    ocstore_releases_dir: "releases"
    ocstore_current_dir: "current"
    
    ocstore_remove_rolled_back: yes
    
    ocstore_rollback_to_release: ""

## License

MIT / BSD

## Author Information

This role was created in 2017 by Alexander Kapitman
