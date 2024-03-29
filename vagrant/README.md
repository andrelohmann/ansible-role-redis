# Test your role with vagrant

Test your role with vagrant

## Prerequisites

  * Virtualbox is installed
  * Vagrant is installed
  * vagrant up will install vagrant-hostmanager module

## Test process

```
cd vagrant
vagrant up
```

The vagrant role will be applied automatically during the vagrant up process.

### Test with molecule from inside vagrant

```
vagrant ssh
cd /etc/ansible/roles/ansible-role- [TAB]
molecule test --all
```

### Test the installation

Ssh into the machine and rund the redis-cli PING command.

```
redis-cli -a r3dis-s3cr3t -h localhost -p 6379 PING
```
