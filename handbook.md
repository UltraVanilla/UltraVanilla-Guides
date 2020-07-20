### Coreprotect

`/fixcreeper <time>` Fixes creeper damage.

`/permaban <player>` Permanently bans a player by banning their account and IP as well as rolling back everything they’ve done for 99 weeks.

### Permission

`/promote <player>` Promotes a player to the next rank.

`/dpromote <player>` Promotes a donator to the next rank.

`/setgroup <player> <rank>` Set a player to a specific rank.

### Player info

`/seen <player> [first]` Check when a player was first or last seen.

`/inv <player> [enderchest]` Open a player’s inventory if they are online. Add ‘enderchest’ to the end of the command to open their ender chest.

`/echest <player>` Opens a player's enderchest.

`/whois <player|nickname>` Use this to find out the username of a nickname is, as well as finding out what role a player has.

`/role <player>` Shows info on a player’s role.

### Misc

`/setlore <line1>[|line2][|line3]...` Add lore to an item. Separate lines with '|'.

`/title [title] [-s <subtitle>] [-to <player>]` Shows a title to all players unless specified using ‘-to’. Use '-s' to specify a subtitle (smaller text).

`/raw <"message"> [-suggest|-command <"command"> | -link <"url">] [-hover <"hover message">] [-to <player>] [+ [...]]` Send a raw message. Concatenate with ‘+’.
	Example:`/raw "Click " + "HERE" -command "hello" -hover "this text is shown only over the HERE" + " to say hello!"` 

`/print <message>` Prints a message that only you can see.

`/do <"command 1"> ["command 2"] ["command 3"]...` Execute multiple commands at once. Do not include a / unless you want to execute //command.

### Navigation

`!` or `/unstuck` will get you out of a block if you somehow got embedded inside.

`/j` or `/jumpto` sends you to the top of the block that you are looking at. If that block is a vertical wall, you will be placed on top of the cliff at the very edge.

`/thru` sends you through a wall in the direction you are looking.

`/ascend [levels]` and `/descend [levels]` let pass through the ceiling above or floor below you. For example, if you were in a skyscraper on the bottom floor, and used `/ascend 2`, you’d be on the 3rd floor.

`/ceil [clearance]` brings you up to the ceiling of the current room that you are in. If you provide no clearance parameter to use, you will be right up to the ceiling. If you do specify a clearance, the space above your head will be larger. 

`/up <distance>` This will move you up a certain number of blocks.
