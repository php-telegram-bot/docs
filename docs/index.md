# Welcome to the PHP Telegram Bot Documentation
<p align="center">
==^^This is a pure PHP Telegram Bot, fully extensible via plugins.^^==
</p>

Telegram announced official support for a Bot API in 2015 allowing integrators of all sorts to bring automated interactions to the mobile platform. This framework aims to provide a platform where one can simply write a plugin and have interactions in a matter of minutes.

The framework can:

* retrieve updates with webhook and getUpdates methods.
* supports all types and methods according to Telegram API (25 May 2016).
* supports supergroups.
* handle commands in chat with other bots.
* manage Channel from the bot admin interface.
* full support for inline bots.
* inline keyboard.
* Messages, InlineQuery and ChosenInlineQuery are stored in the Database.
* Botan.io integration and database cache system. (new!)
Conversation feature

!!! info "Framework status"
    <p align="center">
    [![Join the bot support group on Telegram](https://img.shields.io/badge/telegram-@PHP__Telegram__Bot__Support-32a2da.svg)](https://telegram.me/PHP_Telegram_Bot_Support)
    [![Donate](https://img.shields.io/badge/%F0%9F%92%99-Donate-blue.svg)](#donate)
    <p align="center">
    [![Build Status](https://travis-ci.org/php-telegram-bot/core.svg?branch=master)](https://travis-ci.org/php-telegram-bot/core)
    [![Code Coverage](https://img.shields.io/scrutinizer/coverage/g/php-telegram-bot/core/develop.svg?style=flat-square)](https://scrutinizer-ci.com/g/php-telegram-bot/core/?b=develop)
    [![Code Quality](https://img.shields.io/scrutinizer/g/php-telegram-bot/core/develop.svg?style=flat-square)](https://scrutinizer-ci.com/g/php-telegram-bot/core/?b=develop)
    [![Latest Stable Version](https://img.shields.io/packagist/v/Longman/telegram-bot.svg)](https://packagist.org/packages/longman/telegram-bot)
    [![Total Downloads](https://img.shields.io/packagist/dt/Longman/telegram-bot.svg)](https://packagist.org/packages/longman/telegram-bot)
    [![Downloads Month](https://img.shields.io/packagist/dm/Longman/telegram-bot.svg)](https://packagist.org/packages/longman/telegram-bot)
    [![Minimum PHP Version](http://img.shields.io/badge/php-%3E%3D5.6-8892BF.svg)](https://php.net/)
    [![License](https://img.shields.io/packagist/l/Longman/telegram-bot.svg)](https://github.com/php-telegram-bot/core/LICENSE.md)
    </p>

!!! bug "Github Repository"
    :construction: The code is available on [Github](https://github.com/php-telegram-bot/core), pull request and donations are welcome to keep up and kicking the project. :construction:

??? info "Donations :point_down: "
    All work on this bot consists of many hours of coding during our free time, to provide you with a Telegram Bot library that is easy to use and extend.
    If you enjoy using this library and would like to say thank you, donations are a great way to show your support.

    Donations are invested back into the project :+1:

    - Gratipay: [Gratipay/PHP-Telegram-Bot]
    - Liberapay: [Liberapay/PHP-Telegram-Bot]
    - PayPal: [PayPal/noplanman] (account of @noplanman)
    - Bitcoin: [166NcyE7nDxkRPWidWtG1rqrNJoD5oYNiV][bitcoin]
    - Ethereum: [0x485855634fa212b0745375e593fAaf8321A81055][ethereum]


[Gratipay/PHP-Telegram-Bot]: https://gratipay.com/PHP-Telegram-Bot "Donate with Gratipay"
[Liberapay/PHP-Telegram-Bot]: https://liberapay.com/PHP-Telegram-Bot "Donate with Liberapay"
[PayPal/noplanman]: https://paypal.me/noplanman "Donate with PayPal"
[bitcoin]: bitcoin:166NcyE7nDxkRPWidWtG1rqrNJoD5oYNiV "Donate with Bitcoin"
[ethereum]: https://www.myetherwallet.com/?to=0x485855634fa212b0745375e593fAaf8321A81055 "Donate with Ethereum"
