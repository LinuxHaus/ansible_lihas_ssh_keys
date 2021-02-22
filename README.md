# Role Name

deploy and/or remove specific ssh keys

## Requirements

Uses lihas_variables to determine which keys to use

To run solo:
```
ansible-galaxy install -r requirements.yml
ansible-playbook -i localhost, ssh_keys.yml
```

## Role Variables
`%.config` describes any of the lihas_variables config trees, replace % by anything legal in YAML in your host_vars or group_vars
### %.config.ssh.keys_active.keys: []
List of verbatim keys to activate
### %.config.ssh.keys_inactive.keys: []
List of verbatim keys to deactivate

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## License

GPLv3+

## Author Information

LiHAS, Adrian Reyer <lihas@lihas.de>
