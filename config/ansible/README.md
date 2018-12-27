# How to use

install requirements
```bash
$ ansible-galaxy install -r requirements.yml -p ./roles/vendor
```

edit config file in `group_vars`

deployment server environment
```bash
$ ansible-playbook -i staging site.yml -t init,nginx,postgresql...
$ ansible-playbook -i production site.yml -t all
```
