# vagrant-cactus
Vagrant box for the static site generator Cactus

## Dependencies:

- [Vagrant](https://www.vagrantup.com)
- [Virtualbox](https://www.virtualbox.org)

## How-To

**Clone this repo**
```cmd
git clone https://github.com/fredbourni/vagrant-cactus.git
```
**Start the VM**
```cmd
cd vagrant-cactus
vagrant up
```
**Start the VM**
```cmd
cd vagrant-cactus
vagrant up
```

**Connect to the VM**

- Use Putty or any other SSH client using `127.0.0.1` port `2222`

**Create your first Cactus site**

```bash
cactus create /projects/mysite.com
cd /projects/mysite.com
```

**Test your fresh new site**

```bash
cactus serve
```

This cactus command will start  a python-based Web server you can visit at this address: [http://127.0.0.1:8000/](ttp://localhost:8000/)

## Documentation

- [Cactus](http://cactusformac.com/docs/)
- Django Templates
  - [General](https://docs.djangoproject.com/ja/1.9/ref/templates/language/)
  - [Filters and tags](https://docs.djangoproject.com/en/1.9/ref/templates/builtins/)
- [Vagrant](https://www.vagrantup.com/docs/)
