# Vagrant configuration for java development

`sed -i -e 's/\r$//' wildfly-install.sh` - if problems with new line sybmols occurres

Includes:

1. ubuntu 14
2. wildfly 8.2.1.Final
3. postgres 9.4
4. java 8

Forwarded ports:

    5432 - PostgreSQL
    8080 - WildFly
    9990 - WildFly management console
    8787 - WildFly debug port

To use it just import the box

```
    vagrant box add https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box --name ubuntu/trusty64-cloudimage
```

Initial structure copied from https://github.com/niltsiar/vagrant-ubuntu-14.04-postgresql-9.4-wildfly-8.2/
