!!! summary
    Vagrant is a virtualization software that allows us to create a virtual machine where to run our bot during its development. It's useful mainly for two reasons: it doesn't messes up your own machine and it allows all of us to work with the "same computer" even thought everyone will run it from its own system.


## Download and Install Vagrant

Head to the [download](https://www.vagrantup.com/downloads.html) page to grab and install the appropriate version for your Operating System.

Vagrant needs a file named `Vagrantfile` that containes all the settings\packages etc to prepare the virtual machine that we will be using, luckily enough we prepared a custom one for you to suit our needs. [Download][vagrantfile] it and save it into the `∼Projects` folder.

Now we need to boot up the virtual achine, open a shell and head to the `∼Projects` folder where you saved your `Vagrantfile` to initialize your Vagrant machine:

```shell
$ vagrant up
```

??? Note
    The first time that the command is fired it will takes some time for your machine to be prepared, ensure to have an Internet connection since Vagrant will need to perform:

    * Download of mini version of Ubuntu 16.04
    * Installation of all the dependencies needed by the framework
    * Download (`git clone`) the repository [`example-bot`][example-bot]
    * Initialize the framework through `composer install`
    
...and log into it:


```shell
$ vagrant ssh
```




Install all the required dependencies for our framework to work.

Run the following in the shell:

```shell
sudo apt install php7.0 php7.0-mbstring php7.0-mysql php-curl php-xml mysql-client mysql-server composer git
```





<!-- snippets -->
--8<-- 'linkIndex.md'
