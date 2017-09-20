!!! summary
    In this part of the Documentation we will encounter:

    **Vagrant**
    : A virtualization software that allows us to create a virtual machine where to run our bot during its development. It's useful mainly for two reasons: it doesn't messes up your own machine and it allows all of us to work with the "same computer" even thought everyone will run it from its own system.
    It can be configured with a `Vagrantfile` to setup a predefined custom environment

    **Composer**
    : A package manager which takes care that the framework is kept up-to-date with all its requirements. In this _Let's Play_ part of the guide you won't see it in action since we built-in the `Vagrantfile` the `composer` commands to set up the [`example-bot`][example-bot] during the first boot.

    **Git**
    : A **V**ersion **C**ontrol **S**oftware (VCS), its full usage is beyond the scope of this Documentation at the of its writing. We will just cover few _basic_ commands where needed.



## Initialization of the environment

Head to the [download](https://www.vagrantup.com/downloads.html) page to grab and install the appropriate version for your Operating System.

Vagrant needs a file named `Vagrantfile` that containes all the settings to prepare the virtual machine that we will be using, luckily enough we prepared a custom one for you to suit our needs. [Download][vagrantfile] it and save it into the `∼Projects` folder.

Now we need to boot up the virtual achine, open a shell and head to the `∼Projects` folder where you saved your `Vagrantfile` to initialize your Vagrant machine:

```shell
$ vagrant up
```

??? Note
    The first time that the command is fired it will takes some time for your machine to be prepared, ensure to have an Internet connection since Vagrant will:

    * Download a mini version of Ubuntu 16.04 LTS
    * Install all the dependencies needed by the `php-telegram-bot` framework
    * Download (`git clone`) the repository [`example-bot`][example-bot] to the virtual machine
    * Initialize the framework through `composer install`


Once Vagrant finish the boot up process you can login into the virtual machine by:


```shell
$ vagrant ssh
```


!!! success "If everything went as expected..."

     you will now have the [`example-bot`][example-bot] in your main directory and everything is ready to be configured for actual usage.

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
