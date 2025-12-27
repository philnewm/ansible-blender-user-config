# Blender-user-config-Role

[![Alma9-CI](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/alma9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/alma9-ci-caller.yml) [![Rocky9-CI](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/rocky9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/rocky9-ci-caller.yml) [![CentOSStream9-CI](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/centosstream9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/centosstream9-ci-caller.yml) [![Fedora43-CI](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/fedora43-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/fedora43-ci-caller.yml)<br>
[![Ubuntu2404-CI](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/ubuntu2404-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/ubuntu2404-ci-caller.yml) [![Debian13-CI](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/debian13-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-blender-user-config/actions/workflows/debian13-ci-caller.yml)

Role description

This role includes a molecule testing setup as a submodule at `molecule/`

## Structure

```code
📦 ansible-blender-user-config
 ┣ 📂 defaults
 ┃ ┗ 📜 main.yml
 ┣ 📂 meta
 ┃ ┗ 📜 main.yml
 ┣ 📂 molecule
 ┃ ┗ 📂 default
 ┃   ┗ 📜, 📜, 📜, scenario_files
 ┣ 📂tasks
 ┃ ┣ 📜absent.yml
 ┃ ┣ 📜config.yml
 ┃ ┣ 📜development_setup.yml
 ┃ ┣ 📜main.yml
 ┃ ┣ 📜present.yml
 ┃ ┗ 📜tests.yml
 ┗ 🗒️ README.md
 ┗ 📓 requirements.yml

```

Describe and explain role structure.

## Requirements

Elaborate external dependencies and how to use them.

## Role Variables

* defaults/main.yml
  * first_var
  * sec_var
  * third_var
* vars/main.yml
  * first_var
  * sec_var
  * third_var

## Dependencies

* [philnewm.blender](https://galaxy.ansible.com/ui/standalone/roles/philnewm/blender/)

## Example Playbook

```yaml
---

tasks:
  - name: Include ansible-blender-user-config present
    ansible.builtin.include_role:
      name: ansible-blender-user-config
    vars:
      state: present
      pipeline_dev: true
      user: "ansible"

...
```

## License

Add license - if any.
