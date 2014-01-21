# Ansible Playbooks

## Read first

Don't use any of this playbooks in production, this is just for replicating a _standard_ production host. Some of them exist just for fun :)

## Ansible

Python + ssh = happiness

* [Documentation](http://docs.ansible.com/)

## Vagrant
### Dirty testing

Virtual machine + Ruby = ....

![webscale-everywhere](http://what-if.xkcd.com/imgs/a/20/diamond_11.png)

* [Documentation](http://docs.vagrantup.com/v2/)

To quickly run some playbook on a fresh vagrant I use a `Rakefile`, there is a sample [here](https://github.com/Awea/ansible-playbooks/blob/master/sample.Rakefile).

```ruby
# run it !
rake test
```

### vre alias
#### zsh ftw !

```shell
# Vagrant aliases
alias vdf="vagrant destroy -f"
alias vup="vagrant up"
alias vre="vdf && vup"
```