# Feather-PD2
Lightweight lootfilter for Project Diablo II

This filter is less strict than most and has all the usual improvements, so it's ideal for new players. It's also great for experienced players who like the simple aesthetic of the original game. Multiple strictness levels are available to help the filter better match your preferences.

### Design
The game's original aesthetic is preserved as much as possible without sacrificing functionality.
* Highlighting is accomplished with space rather than extra colors or symbols.
* Item tooltips only include extra info when it's especially relevant, and are otherwise kept relatively simple to reduce clutter and improve readability.
* Info which only needs to be referenced infrequently is displayed on the "extra info" filter level alone - it can be quickly toggled on/off without adding clutter during regular gameplay.

The filter's strictness is designed to be minimally intrusive.
* It focuses on hiding the minimum amount of items to prevent random items from disappearing due to the game's item limit.
* Each filter level hides groups of increasingly uncommon and/or useful items (listed [below](https://github.com/BetweenWalls/Feather-PD2#Filter_Versions)) so that players can better understand exactly what is and isn't hidden.
* The choice of what to pick up is still largely in the hands of the player - the filter avoids making decisions about what is worthy and what isn't by hiding relatively few items and using notifications sparingly.

### Features
* non-equipment more clearly distinguished from equipment (potions, gems, jewels, charms, maps)
* item highlighting and notifications for more useful/valuable items
* item info displayed (ethereal/socketed/superior/automods/skillmods)
* descriptions for equipment recipes, maximum possible sockets, possible runewords, set bonuses, socketed gem/rune effects, item price
* shopping for valuable items made easier
* and more...

### Filter Versions
Some characters and colors only work if HD text is enabled - if you have it disabled, use **feather-old-text.filter**.
| Version | Description |
| --- | --- |
| feather.filter | teal charms & "middle dot" characters for pointmod items
| feather-old-text.filter | purple charms & "soft hyphen" characters for pointmod items

### Filter Levels
| Level | Name | Description |
| --- | --- | --- |
| 1 | Min&nbsp;Strictness&nbsp;(Extra&nbsp;Info) | Same as "Minimum Strictness" but items include extra info like crafting info, rune combinations for runewords, set bonuses, weapon speed/range, map immunities, extra recipes, etc
| 2 | Minimum Strictness | Shows all magic equipment and most regular equipment, includes notifications for more items than higher filter levels<br><br>Hides some basic non-equipment items and useless equipment:<br>&#x2022; tiny gold piles<br>&#x2022; low-level potions<br>&#x2022; low-level gems<br>&#x2022; scrolls<br>&#x2022; keys<br>&#x2022; most regular non-class items which can never be used for runewords<br>&#x2022; most regular skill-capable items which don't have skills
| 3 | Low Strictness | Hides additional items which are only useful in very niche cases and are widely ignored:<br>&#x2022; inferior items<br>&#x2022; magic quivers<br>&#x2022; the worst non-class magic bases<br>&#x2022; the worst "plain" non-class regular bases which aren't ethereal/superior/socketed<br>&#x2022; some regular items with bottom-tier automods
| 4 | Moderate Strictness | Hides additional items:<br>&#x2022; gold piles below 1000<br>&#x2022; magic rings<br>&#x2022; many non-elite magic items which can be purchased from vendors<br>&#x2022; the worst non-class normal/exceptional regular bases which aren't at least 2 of: ethereal/superior/socketed<br>&#x2022; a few of the very worst regular elite weapons
| 5 | High Strictness | Hides additional items:<br>&#x2022; gold piles below 2000<br>&#x2022; most normal magic non-class armors<br>&#x2022; magic non-eth normal non-class throwing weapons<br>&#x2022; normal "plain" or 2-socket regular non-class items
| 6 | Severe Strictness | Hides additional items:<br>&#x2022; gold piles below 3000<br>&#x2022; super potions<br>&#x2022; most exceptional magic non-class armors<br>&#x2022; magic non-eth exceptional non-class throwing weapons<br>&#x2022; exceptional "plain" or 2-socket regular non-class items<br>&#x2022; most regular non-elite class items with only +1 to any skill unless they match the character's class
| 7 | Extreme Strictness | Hides additional items:<br>&#x2022; gold piles below 5000<br>&#x2022; small rejuvation potions<br>&#x2022; magic amulets<br>&#x2022; most magic non-class armors<br>&#x2022; many magic non-elite class items which don't match the character's class<br>&#x2022; all "plain" or 2-socket regular non-class items<br>&#x2022; most regular non-elite class items with only +2 to any skill unless they match the character's class<br>&#x2022; most regular elite class items with only +1 to any skill unless they match the character's class

Nothing is hidden at character level 1 - items become hidden as the character levels up and progresses through the game. Many items aren't hidden at all until level 70-80 in Hell difficulty, for example.

The following items are never hidden:
* rare, crafted, set, and unique items
* ethereal magic items
* identified items of magic rarity or higher
* items in town
* any items that that aren't listed in the above "Filter Levels" chart

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

Some older images are included below:

![_](/images/unidentified_highlighting.png)

![_](/images/regular_items.png)

![_](/images/potions_and_stuff.png)

![_](/images/runes.png)
