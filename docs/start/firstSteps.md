# First steps with the "plug-n-play" example-bot

## Grab a copy of the example-bot

If you know your way around `git` you can clone the master repository to your _local development environment_:

```
$ git clone https://github.com/php-telegram-bot/example-bot.git
```

If you don't know\don't want to use `git` you can download it as a `.zip` and then extract it in your Project folder:

* either via direct [download](https://github.com/php-telegram-bot/example-bot/archive/master.zip)
* or via `curl`:

```
$ curl -o example-bot.zip https://github.com/php-telegram-bot/example-bot/archive/master.zip
```

!!! summary "Your directory will now look like this"
    ```
    .
    ├── Commands
    ├── composer.json
    ├── cron.php
    ├── getUpdatesCLI.php
    ├── hook.php
    ├── LICENSE
    ├── manager.php
    ├── README.md
    ├── set.php
    └── unset.php

    1 directory, 10 files
    ```


**We can now get our hands dirty with few real coding parts!**


## Configuring the bot with your credentials


!!! important
    Telegram supports **two** different methods to "talk" with your bot, they are referred as _Webhook_ and _getUpdates_. The main difference is that with the former Telegram servers send updates to your bot while with the latter it's your bot that asks for them.

    We will first go through the _getUpdates_ method for developing locally and then we will switch to the _Webhook_ — yes it will be as easy as flipping a switch.


## :point_right: getUpdatesCLI installation

!!! info
    This configuration is suggested for a _local development environment_ as it is **way easier** to setup and yet very effective. When switching to a _remote host_ the Webhook performs better, at that a proper time the method will be explained and implemented.


Open your `getUpdatesCLI.php` with any text editor and modify these lines with your bot credentials:

```php linenums="15"
// Add you bot's API key and name
$bot_api_key  = 'your:bot_api_key';
$bot_username = 'username_bot';
```



Now head to the very end of the file and add:

 `sleep(3); // Make the script sleep for three seconds`







 Here we go, the `example-bot` is now ready to be fired up! :fire:


### Testing the example-bot

 So far so good,

 ---

## :point_right: Webhook installation

!!! attention
    From now on the Documentation will assume that you are using the installation with the `manager.php` functionality. If you followed the previous steps, you're fine and you don't have to worry about it since the `example-bot` already comes shipped with it.


## Meet the manager!

!!! info
    `manager.php` is a special file that can handles different management task for our bot as shown later. It is most useful when your bot lives online on a remote VPS.

!!! warning
    While developing your bot in your _local development enviroment_ `manager.php` has no real use.
    Skip to [Configure getUpdatesCLI.php](#configure-getupdatescli)

 The bare minimum setup for `manager.php` is the following, where you need to replace the `'api_key'`, `'bot_username'`, `'secret'` and `'webhook'` values with your own.
