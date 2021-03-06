# VictorySlot

 [VCASH](https://github.com/openvcash/vcash) based slot game.

## Requirements

* WINDOWS: WAMP server environment
* LINUX: LAMP server environment

## Installation

* Create database by the script [create_db.sql](src/db/create_db.sql)
* Copy the files from src folder to your server
* Set up the database access configuration in [Config.php](src/include/Config.php)
* Install VCASH daemon on your server

## Components

Slot values are generated by [SlotGame.php](src/include/SlotGame.php) file functions  
The game follows the payout rules of a fruit slot from http://wizardofodds.com/games/slots/appendix/4/

[VcashRpc](src/include/VcashRpc.php) class sends JSON-RPC commands to VCASH daemon or GUI wallet.

[BetDb](src/include/BetDb.php) class contains functions that saves bet data in the database

## Credits

> These projects are used inside VictorySlot

* JQuery "Slot Machine Construction Kit" 
[ezSlots](https://github.com/kirkjerk/ezslots)
* A simple PHP CAPTCHA script
[simple-php-captcha](https://github.com/claviska/simple-php-captcha)
* JSON RPC eXtended
[jsonrpcx-php](https://github.com/jenolan/jsonrpcx-php)
