# ScoreboardsDX
ScoreboardDX plugin used by dctxgames to create scoreboards
# Features:
- create Scoreboards
- Virion Support (at the second branch)
- Plugin Support (you currently at the plugins branch)
# example of creating an scoreboard for your minigame
usage:
```php
<?php

use Scoreboards\Scoreboards;
```
Creating The Scoreboard:
```php
  $api = Scoreboards::getInstance();
  $api->new($player, "ObjectiveName", "§l§eEXAMPLE MINIGAME");
  $api->setLine($player, 1, "§7" . date("d/m/Y"));
  $api->setLine($player, 2, "  ");
  $api->setLine($player, 3, "Map: §a";
  $api->setLine($player, 4, "   ");
  $api->setLine($player, 5, "Players: §a2/2");
  $api->setLine($player, 6, "      ");
  $api->setLine($player, 7, "Starting in §a0");
  $api->setLine($player, 8, "          ");
  $api->setLine($player, 9, "§ewww.servername.com";
```
Removing The Scoreboard:
```php
    if(Scoreboards::getInstance()->getObjectiveName($player)){
				Scoreboards::getInstance()->remove($player);
		}
```
-----------
By DctxGamesMC
- ItzToxicGG
- DanteDev
