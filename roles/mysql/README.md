# Install MySQL

Install MySQL (MariaDB) on CentOS

# Variables

MySQL root password You can change in vars. Many variables and info about it see in ```var/main.yml```


# Use in playbook

```yaml
  roles:
    - { role: mysql, action: 'install', root_db_password: 'rootpass' }
    - { role: mysql, action: 'create-database', database_name: 'db_name' }
    - { role: mysql, action: 'create-user',  database_user: 'test', database_password: 'test' }
```
                                                                                
Avaible action:

- *install* - install MySQL server and configure
- *create-database* - create database
- *create-user* create user

# Dependencies

None

# License 

BSD

# Athor

Igor Bronovskyi - @[BrunIF](https://github.com/BrunIF)

Twitter: @[BrunIF](https://twitter.com/BrunIF)

FB: [BrunIF](https://fb.com/BrunIF)

VK: [BrunIF](https://vk.com/BrunIF)

