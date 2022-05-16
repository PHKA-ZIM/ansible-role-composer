# Composer automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-composer
  name: ansible-role-composer
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-composer

- Import role and override role variables, e.g.
```
- name: Setup composer
  roles:
    - role: ansible-role-composer
```

- All available role vars can be found in `defaults`
