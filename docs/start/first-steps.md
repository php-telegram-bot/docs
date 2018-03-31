# First steps with the "plug-n-play" example-bot

## Configuring the bot with your credentials


!!! important
    Telegram supports **two** different methods to "talk" with your bot, they are referred as _Webhook_ and _getUpdates_. The main difference is that with the former Telegram servers send updates to your bot while with the latter it's your bot that asks for them.

    We will first go through the _getUpdates_ method for developing locally and then we will switch to the _Webhook_ — yes it will be as easy as flipping a switch.


### :point_right: getUpdatesCLI setup

!!! info
    This configuration is the suggested one for a _local development environment_ as it is **way easier** to setup and yet very effective. When switching to a _remote host_ the Webhook performs better, at a proper time the method will be explained and implemented.


Open your `getUpdatesCLI.php` with any text editor[^1] and modify these lines with your bot credentials:

```php linenums="15"
// Add you bot's API key and name
$bot_api_key  = 'your:bot_api_key';
$bot_username = 'username_bot';
```



Now head to the very end of the file and add:

```php linenums="90"
 sleep(3); // Makes the script sleep for three seconds, let it chill
```

Here we go, the `example-bot` is now ready to be fired up! :fire:


### Preliminary testing of the example-bot

 So far so good, in a shell execute the following command:

```shell
 $ while true; do ./getUpdatesCLI.php; done
```

If everything has been set up right the bot is now running in your virtual machine, open a Telegram chat with it and try the basic command `/whoami`, the bot should answer with your profile picture, id and other infos.

!!! summary "What have we done so far and getUpdatesCLI.php breakdown"
    


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




 [^1]: It **must** support the UTF-8 encoding, if you don't know what I'm talking about chances are you are good with your editor since it's the default 99% of the time.
