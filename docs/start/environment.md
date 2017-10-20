!!! summary
    In this part of the Documentation we will encounter:

    **Vagrant**
    : A virtualization software that allows us to create a virtual machine where to run our bot during its development. It's useful mainly for two reasons: it doesn't messes up your own machine and it allows all of us to work with the "same computer" even thought everyone will run it from its own system.
    It can be configured with a `Vagrantfile` to setup a predefined custom environment

    **Composer**
    : A package manager which takes care that the framework is kept up-to-date with all its requirements. In this _Let's Play_ part of the guide you won't see it in action since we built-in the `Vagrantfile` the `composer` commands to set up the [`example-bot`][example-bot] during the first boot.

    **Git**
    : A **V**ersion **C**ontrol **S**oftware (VCS), its full usage is beyond the scope of this Documentation at the time of its writing. We will just cover few _basic_ commands where needed.



## Initialization of the environment

### :point_right: Vagrant Install
Head to the [download](https://www.vagrantup.com/downloads.html) page to grab and install the appropriate version of Vagrant for your Operating System.

Vagrant needs a file named `Vagrantfile` that contains all the settings to prepare the virtual machine that we will be using, luckily enough we prepared a custom one for you to suit the framework needs.

### :point_right: Download the example-bot
Download and unzip the [`example-bot`][example-bot] into your `∼Projects` folder.

### :point_right: First Virtual Machine boot
Now we need to boot up the virtual machine, open a shell and head to the `∼Projects` folder where you saved your `Vagrantfile` to initialize your Vagrant machine with:

```shell
$ vagrant up
```

??? Note
    The first time that the command is fired it will takes some time for your machine to be prepared, ensure to have an Internet connection since Vagrant will:

    * Download a mini version of Ubuntu 16.04 LTS
    * Install all the dependencies needed by the `php-telegram-bot` framework
    * Initialize the framework through `composer install`
    * Set up a basic MySQL database with mandatory pre-prepared tables for the framework usage.


Once Vagrant finish the boot up process you can login into the virtual machine with:


```shell
$ vagrant ssh
```


!!! success "If everything went as expected..."

     ...you will now have the `example-bot` in your main directory as in the example below and everything is ready to be configured for actual usage.

    ```shell
    vagrant@vagrant:~$ tree -L 2
    .
    └── example-bot
        ├── Commands
        ├── composer.json
        ├── composer.lock
        ├── cron.php
        ├── getUpdatesCLI.php
        ├── hook.php
        ├── LICENSE
        ├── manager.php
        ├── README.md
        ├── set.php
        ├── unset.php
        └── vendor

    3 directories, 10 files
    ```




<!-- snippets -->
--8<-- 'linkIndex.md'
