### Aspnet vnext virtual machine

1. [install vagrant](http://docs.vagrantup.com/v2/installation)
2. [install ansible](http://docs.ansible.com/intro_installation.html)
3. add box to your local, reusable box repository (can take a wile or more)
    
  3.1 use: ```vagrant box add janihur/ubuntu-1404-desktop```

  3.2 or: ```vagrant box add https://atlas.hashicorp.com/janihur/ubuntu-1404-desktop```

4. clone this repo
5. from project folder, run: ```vagrant up``` them ```vagrant provision```
