# Feather-PD2
Lootfilter for Project Diablo II

This is a minimally-strict filter that includes many quality-of-life features. Few items are hidden, but enough is hidden that the onscreen-item-limit rarely comes into play.

If you prefer to see fewer items, some rules are included that, when enabled, will increase the filter's strictness substantially for higher level characters.

## Features
* mostly follows classic style (it still looks like D2)
* non-equipment more clearly distinguished from equipment (gems, jewels, charms)
* items highlighted based on their usefulness
* notifications for valuable items
* item info (ethereal/socketed/superior/automods/skillmods) displayed
* shopping for valuable items made easier
* descriptions for socketed effects on stacked gems/runes
* descriptions for possible runewords
* descriptions for craft/upgrade/socket/reforge/repair recipes where appropriate
* descriptions for maximum possible sockets where appropriate
* descriptions for item price on regular/magic/rare items

#### Hidden Items:
Nothing is hidden at level 1 - items become hidden as the character levels up.
* basic non-equipment: smaller gold piles, low-level potions, low-level gems, scrolls, keys
* regular items that have zero use for runewords
* regular skill-capable items without skills
* some of the worst regular/magic equipment bases

## Installation
This filter is included in the [launcher](https://github.com/Project-Diablo-2/LootFilters#project-diablo-2-loot-filters). To install manually, download [**loot.filter**](https://github.com/BetweenWalls/Feather-PD2/blob/main/loot.filter) (right-click [**Raw**](https://raw.githubusercontent.com/BetweenWalls/Feather-PD2/main/loot.filter) & select **Save link as**) and save it to *Diablo II\ProjectD2*. In order to access it from the launcher, save it to *Diablo II\ProjectD2\filters\local* instead.

Once in-game, enable these options from the *Settings* menu:
* Advanced Item Display
* Item Drop Notifications
* Item Close Notifications
* Item Detailed Notifications

If you copy/paste the filter's *raw text*, some characters may be displayed incorrectly - the file uses ANSI encoding instead of standard UTF-8 encoding. Either download the file normally, [download everything](https://github.com/BetweenWalls/Feather-PD2/archive/main.zip) and extract the file, or copy/paste the [*encoded text*](https://github.com/BetweenWalls/Feather-PD2/blob/main/loot.filter) into a file that uses ANSI encoding.
<!--## Images
![_](/images/regular_items.png)
![_](/images/runes.png)
![_](/images/unidentified_highlighting.png)-->
