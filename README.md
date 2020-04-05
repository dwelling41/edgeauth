## Running the unit tests
1. Make sure you have composer installed on your computer (https://getcomposer.org/download/)
2. In this directory run `composer install`
3. In this directory run `composer run unit`

## Installing in an existing app with an autoloader
1. Copy the files under Src/ into a folder at your root named EdgeAuth and things will just work. If you want to change the folder location, you just need to update the namespace of both DigestTokens.php and TokenBuilder.php accordingly.

## Installing in an existing app without an autoloader
1. Copy the files under Src/ into a folder of your choosing
2. Wherever you choose to use the files, require them with:
```
<?php 

require_once __DIR__ . '/path/to/files/DigestTokens.php'
require_once __DIR__ . '/path/to/files/TokenBuilder.php'
```

## Usage
1. The library follows the same fluent interface that was implemented in the node library. See Examples\App.php and Test\DigestTokensTest for examples

