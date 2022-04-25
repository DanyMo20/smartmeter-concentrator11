This project was moved to https://gitlab.ics.muni.cz/muni-kypo/ansible-roles/disable-qxl.

# Ansible role - Disable QXL

This role disables kernel module QXL and restarts the target machine. Tested only on Debian-like operating systems.

## Requirements

* This role requires root access, so you either need to specify `become` directive as a global or while invoking the role.

    ```yml
    become: yes
    ```
    
* Also requires Ansible variables, therefore do not disable directive `gather_facts`.

## Role parameters

No parameters

## Example

Example of the simplest QXL module disabling.

```yml
roles:
    - role: kypo-disable-qxl
      become: yes
```
