!!! summary
    Vagrant is a virtualization software that allows us to create a virtual machine where to run our bot during its development. It's useful mainly for two reasons: it doesn't messes up your own machine and it allows all of us to work with the "same computer" even thought everyone will run it from its own system.


## Download and Install Vagrant

Head to the [download](https://www.vagrantup.com/downloads.html) page, grab and install the appropriate version for your Operating System.
Once you are done open a shell and head to the `∼Projects` folder to initialize your Vagrant machine:

```shell
$ vagrant init ubuntu/xenial64
```

Once your _virtual environment_ is ready we need to "boot" with:

```shell
$ vagrant up
```

...and log into it:


```shell
$ vagrant ssh
```




Install all the required dependencies for our framework to work.

Run the following in the shell:

```shell
sudo apt install php7.0 php7.0-mbstring php7.0-mysql php-curl php-xml mysql-client mysql-server composer git
```
