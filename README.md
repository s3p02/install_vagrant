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

# Suspend machine

```
vagrant suspend machine_name
```

# List all VM'm on host

```
vagrant global-status
```

Above command lists information about all known Vagrant environments on this machine. This data is cached and may not be completely up-to-date. To interact with any of the machines, you can go to that directory and run Vagrant, or you can use the ID directly with Vagrant commands from any directory. For example:"vagrant destroy __GLOBAL__ID__"

# Copy file from host to machine

```
vagrant scp /path/to/file/on/host/ __GLOBAL__ID__:/home/vagrant/
```

# Permanantly Destroy your VM

Suspend or stop your VM first.

```
vagrant destroy __GLOBAL__ID__
```


