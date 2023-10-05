# Feather-PD2
Lightweight lootfilter for Project Diablo II

This filter is less strict than most and has all the usual improvements, so it's ideal for new players. It's also great for experienced players who like the simple aesthetic of the original game. Multiple strictness levels are available to help the filter better match your preferences.

### Design
The game's original aesthetic is preserved as much as possible without sacrificing functionality - highlighting is accomplished with space rather than extra colors or symbols. Item tooltips only include extra info when it's especially relevant, and are otherwise kept relatively simple to reduce clutter and improve readability. Info which only needs to be referenced infrequently is only displayed when the "extra info" filter level is enabled - it can be quickly toggled on/off without adding clutter during regular gameplay.

The filter's strictness is designed from the bottom up - the lowest filter levels are "minimally" strict and focus on hiding just enough items to prevent random items from disappearing due to the game's item limit. The choice of what to pick up is still largely in the hands of the player - the filter avoids making decisions about what is worthy and what isn't by hiding as few items as possible. Successive filter levels each expand the number of hidden items, and the highest level hides a surprisingly large percentage of total items for how relaxed it still is. The slow increase in strictness between filter levels should make it easier for players to tune into their preferences as well as give them a strong foundation for gauging the strictness of other filters.

### Features
* non-equipment more clearly distinguished from equipment (potions, gems, jewels, charms, maps)
* item highlighting and notifications for more useful/valuable items
* item info displayed (ethereal/socketed/superior/automods/skillmods)
* descriptions for equipment recipes, maximum possible sockets, possible runewords, socketed gem/rune effects, item price, etc
* shopping for valuable items made easier
* a lot more... 

### Filter Versions
Some characters and colors only work if HD text is enabled - if you have it disabled, use **feather-old-text.filter**.
| Version | Description |
| --- | --- |
| feather.filter | teal charms & "middle dot" characters for pointmod items
| feather-old-text.filter | purple charms & "soft hyphen" characters for pointmod items

### Filter Levels
| Level | Name | Description |
| --- | --- | --- |
| 1 | Min&nbsp;Strictness&nbsp;(Extra&nbsp;Info) | Same as "Minimum Strictness" but items include extra info like rune combinations for runewords, set bonuses, weapon speed/range, map immunities, extra recipes, etc
| 2 | Minimum Strictness | Shows all magic equipment and most regular equipment, includes notifications for more items than higher filter levels<br>Hides tiny gold piles, low-level potions, low-level gems, scrolls, keys, and useless equipment: most regular items that can never be used for runewords, most regular skill-capable items that don't have skills, and some regular items with bottom-tier automods
| 3 | Low Strictness | Hides many items which are only useful in very niche cases and are widely ignored: inferior items, magic quivers, and the worst regular/magic bases
| 4 | Moderate Strictness | Hides gold piles below 1000, most magic normal armor, and most regular non-elite plain normal items
| 5 | High Strictness | Hides gold piles below 1500, magic normal/exceptional non-eth weapons, and most magic chests/shields
| 6 | Severe Strictness | Hides gold piles below 2000, super potions, nearly all regular plain items, and most regular/magic normal class items that don't match the character's class
| 7 | Extreme Strictness | hides gold piles below 5000, small rejuvation potions, and most exceptional regular/magic normal class items that don't match the character's class

Nothing is hidden at character level 1 - items become hidden as the character levels up and progresses through the game. Many items aren't hidden at all until level 70-80 in Hell difficulty, for example. Rare/set/unique items are never hidden, and the same is also true for all identified items of magic rarity or higher.

For a more thorough breakdown of which items are hidden, see the filter file itself - only a handful of rules actually hide anything and they each include a short explanation of which items are included and when the rule applies.

### Installation
This filter is included in the [launcher](https://github.com/Project-Diablo-2/LootFilters#project-diablo-2-loot-filters) - just click and play. I recommend using these settings:

![_](/images/settings.png)

The "Show Item Level" option will display redundant ilvl/alvl info if enabled since the filter handles that info itself.

These settings should all be enabled by default:
* Enable Loot Filter
* Drop Notifications
* Close Notifications
* Detailed Notifications

### Editing
To use a local version that will preserve your own changes, either copy the file from *Diablo II\ProjectD2\filters\online\BetweenWalls* to *Diablo II\ProjectD2\filters\local* or download [**feather.filter**](https://github.com/BetweenWalls/Feather-PD2/blob/main/feather.filter) (right-click [**Raw**](https://raw.githubusercontent.com/BetweenWalls/Feather-PD2/main/feather.filter) & select **Save link as**) and save it to *Diablo II\ProjectD2\filters\local*. Local filters are selected from the launcher in the same way that others are.

If you copy/paste the filter's *raw text*, some characters may be displayed incorrectly - the file uses ANSI encoding instead of standard UTF-8 encoding. Either download the file normally, [download everything](https://github.com/BetweenWalls/Feather-PD2/archive/main.zip) and extract the file, or copy/paste the [*encoded text*](https://github.com/BetweenWalls/Feather-PD2/blob/main/feather.filter) into a file that uses ANSI encoding.

### Feedback
Feel free to leave feedback in PD2's [#lootfilter](https://discord.com/channels/701658302085595158/771820538502971402) discord channel. You can also reach me directly on discord (@BetweenWalls) or on reddit ([BetweenWalls](https://www.reddit.com/message/compose/?to=BetweenWalls&subject=Feather-PD2)).

![_](/images/unidentified_highlighting.png)

![_](/images/regular_items.png)

![_](/images/potions_and_stuff.png)

![_](/images/runes.png)
