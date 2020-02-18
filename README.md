# ansible-wp
### For create Database Schema(Collection)

### Setup variable
1. Fix **`hosts file`**
2. Fill specific variable

```bash
[ecs-wp]
<ip server>

[ecs-wp:vars]
login_host= <RDS dns>
login_user= <RDS username>
login_password= <RDS password>
```

3. Run command ansible
```bash
$ ansible-playbook playbooks/create-schema.yml --private-key=<your-privatekey>
```
