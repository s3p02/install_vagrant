# Install Virtual Box

```
sudo apt-get install virtualbox
```

# Install Vagrant

```
sudo apt-get install vagrant
```

# Adding OS

Standard way to add is :

```
vagrant box add __NAME__BOX__ __BOX__URL__
```

[URL's](https://app.vagrantup.com/boxes/search) can be searched from a catalog.

For Ubuntu 14.04

```
vagrant box add ubuntu/trusty64 https://atlas.hashicorp.com/ubuntu/boxes/trusty64/versions/14.04/providers/virtualbox.box
```

# Create a directory for OS

```
mkdir ubuntu14
cd ubuntu
```

Initialize Vagrant File

```
vagrant init ubuntu/trusty64
```

Start VM

```
vagrant up
```

# List running Vagrant VM's

```
vagrant status
```

note the machine_name

# SSH to machine

```
vagrant ssh machine_name
```
