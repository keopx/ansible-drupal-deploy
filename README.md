# Ansistrano for Drupal

## Introduction

This is a base template to deploy drupal sites using Ansible with Ansistrano role.

Check _host_ file to change IP and _deploy.yml_ to modify configuration values.

## Install

```
$ sudo apt-get install ansible
$ sudo ansible-galaxy install ansistrano.deploy ansistrano.rollback
```

### Repository

- https://ansistrano.com/
- https://github.com/ansistrano/deploy
- https://github.com/keopx/ansible-drupal-deploy

## Deploy

### Run Remote

```
$ cd /my-proyect/ansible/
$ ansible-playbook -i hosts deploy.yml
```

### Run local
```
$ cd /var/www/my-app/current/ansible/
$ ansible-playbook -i hosts deploy.yml
```

## Rollback

### Run Remote

```
$ cd /my-proyect/ansible/
$ ansible-playbook -i hosts rollback.yml
```

### Run local
```
$ cd /var/www/my-app/current/ansible/
$ ansible-playbook -i hosts rollback.yml
```
