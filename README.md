# ansible-cfg-mystery

Trying to get ansible-playbook working with a custom roles_path

I generated a role using `ansible-galaxy init test-role-1` under ~/devel/ansible/roles`.
I generated `ansible.cfg` using `ansible-config init --disabled > ansible.cfg` and added `~/devel/ansible/roles` to `roles_path`.

When I run `ansible-playbook playbook.yaml` I get the following error:

```
ERROR! the role 'test-role-1' was not found in....
```

If I put The role under `roles` in this directory the playbook is run fine. 

What am I missing?
