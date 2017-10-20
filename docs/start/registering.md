# Registering your bot

## Meet Botfather

<p align="center">
  <img src="https://core.telegram.org/file/811140327/1/zlN4goPTupk/9ff2f2f01c4bd1b013" width="250">
</p>

Everytime this guy :point_up: get mentioned it's sold like "Create your first bot!". No way. Botfather will not make you a bot _at all_. :punch:

!!! info "Don't get me wrong but..."
    It's more like a _Civil Registry_ of the bots and as such handles our bot **Name**, **Username** and **Token**, that's all. Nothing working will be made through it.


---
**Name**
: It's displayed in contact details and elsewhere.

**Username**
: It's a short name, to be used in @mentions and telegram.me links. Usernames are 5-32 characters long and are case insensitive, but may only include Latin characters, numbers, and underscores. Your bot's username must end in ‘bot’, e.g. ‘tetris_bot’ or ‘TetrisBot’.

**Token**
: It's a string along the lines of `110201543:AAHdqTcvCH1vGWJxfSeofSAs0K5PALDsaw` that is required to authorize the bot and send requests to the Bot API. The token **must** be kept secret, it's like your house keys and whoever has it can steal your bot, but don't worry too much because you can generate a new token anytime.

---

## Create your bot credentials
<!-- gif botfather to insert -->

Open a chat with [@Botfather][botfather], then use the `/newbot` command to commence the procedure to create a new bot. [@Botfather][botfather] will ask you for a **Name** and a **Username**, then it will generate an authorization **Token** for your new bot.
<p align='center'>
**Nice! Your bot is now _registered_ with Telegram.**
</p>

???+ tip
    By default bots can **only** see messages starting with a `/` If you plan to use your bot in groups, you can choose whether to allow it or not to receive *all* the messages sent in the chat.

    ??? info "Set the group privacy"
        Default: `ENABLED`

        Use the `/setprivacy` command to commence the procedure, you will be asked to choose the bot for which you want to modify the privacy then you can choose `DISABLE`.

!!! warning
    Keep these informations available as we will use them later in the actual bot creation.


[botfather]: https://t.me/botfather
