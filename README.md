# Feather-PD2
Lightweight lootfilter for Project Diablo II

This filter is less strict than most and has all the usual improvements, so it's ideal for new players. It's also great for experienced players who like the simple aesthetic of the original game. Multiple strictness levels are available to help the filter better match your preferences.

### Design
The game's original aesthetic is preserved as much as possible without sacrificing functionality - highlighting is accomplished with space rather than extra colors or symbols. Item tooltips only include extra info when it's especially relevant, and are otherwise kept relatively simple to reduce clutter and improve readability. Info which only needs to be referenced infrequently is only displayed when the "extra info" filter level is enabled - it can be quickly toggled on/off without adding clutter during regular gameplay.

The filter's strictness is designed from the bottom up - the lowest filter levels are "minimally" strict and focus on hiding just enough items to prevent random items from disappearing due to the game's item limit. The choice of what to pick up is still largely in the hands of the player - the filter avoids making decisions about what is worthy and what isn't by hiding as few items as possible. Successive filter levels each expand the number of hidden items, and the highest level hides a surprising percentage of total items for how relaxed it still is. The slow increase in strictness between filter levels should make it easier for players to tune into their preferences as well as give them a strong foundation for gauging the strictness of other filters.

### Features
* non-equipment more clearly distinguished from equipment (potions, gems, jewels, charms, maps)
* item highlighting and notifications for more useful/valuable items
* item info displayed (ethereal/socketed/superior/automods/skillmods)
* descriptions for equipment recipes, maximum possible sockets, possible runewords, socketed gem/rune effects, item price, etc
* shopping for valuable items made easier
* a lot more... 

### Filter Levels
| Level | Name | Description |
| --- | --- | --- |
| 1 | Min&nbsp;Strictness&nbsp;(Extra&nbsp;Info) | same as "Minimum Strictness" but items include extra info like rune combinations for runewords, weapon speed/range, map immunities, extra recipes, etc
| 2 | Minimum Strictness | shows all magic equipment and most regular equipment, notifies for more items than higher levels
| 3 | Low Strictness | same as original strictness (before filter levels were introduced)
| 4 | Moderate Strictness | hides larger gold piles and additional regular/magic items at level 80+
| 5 | High Strictness | hides larger gold piles and additional regular/magic items at level 80+ (even more)
| 6 | Maximum Strictness | hides larger gold piles, super potions, and additional regular/magic items at level 90+

### Hidden Items
Nothing is hidden at character level 1 - items become hidden as the character levels up. For a more thorough breakdown of which items are hidden, see the filter file itself - only a handful of rules actually hide anything and they each include a short explanation of which items are included and when the rule applies.
* basic non-equipment: smaller gold piles, low-level potions, low-level gems, scrolls, keys
* regular items that have zero use for runewords
* most regular skill-capable items without skills
* some of the worst regular/magic equipment bases (filter level 2+ only)
* some off-class regular/magic items (filter levels 5+ only)

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
Feel free to leave feedback in PD2's #lootfilter discord channel. You can also reach me directly in discord (@BetweenWalls#2390) or in reddit ([BetweenWalls](https://www.reddit.com/message/compose/?to=BetweenWalls&subject=Feather-PD2)).

![_](/images/unidentified_highlighting.png)

![_](/images/regular_items.png)

![_](/images/potions_and_stuff.png)

![_](/images/runes.png)
