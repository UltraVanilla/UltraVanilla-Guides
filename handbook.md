### A note about how to read this guide:
`<these>` are arguments you MUST include while typing the command, just don’t include the actual `< >` characters.

`[these]` are optional arguments you could include if you wanted to but will not give you an error if you omit. If there is a `…` next to it, it means you can have as many arguments as you like.

`["these"]` and `<"these">` are arguments you must enclose in quotation marks or else! 
	Example: `/command "argument 1" "argument 2"`

Arguments that start with a `-` such as `-s` and `-to` take the argument after it. 
	Example: `/command something -s something else`


The `|` symbol means OR. If it is inside a `[ ]` or `< >` such as `<player|nickname>`, it reads as "player OR nickname".

---

### Coreprotect

`/fixcreeper <time>` Fixes creeper damage.

`/permaban <player>` Permanently bans a player by banning their account and IP as well as rolling back everything they’ve done for 99 weeks.

### Permissions

`/promote <player>` Promotes a player to the next rank.

`/donator <player>` Mark a player as a donator, effectively giving them all donator permissions.

`/setgroup <player> <rank>` Set a player to a specific rank.

### Player info

`/seen <player> [first]` Check when a player was first or last seen. Click on their last location to teleport. 
	Example: `/seen Akoot_ first`

`/inv <player> [enderchest]` Open a player’s inventory if they are online. Add ‘enderchest’ to the end of the command to open their ender chest. 
	Example: `/inv Akoot_ enderchest` (same as `/echest Akoot_`)

`/echest <player>` Opens a player's enderchest.

`/whois <player|nickname>` Use this to find out the username of a nickname is, as well as finding out what role a player has. 
	Example: `/whois Yoda`

`/role <player>` Shows info on a player’s role.

### Misc

`/setlore <line1>[|line2][|line3]...` Add lore to an item. Separate lines with '\|'. 
	Example: `/setlore This sword is quite epic.|The most epic sword I have ever seen.|It is worth a million bucks,|but I'm not allowed to sell it.`

`/title [title] [-s <subtitle>] [-to <player>]` Shows a title to all players unless specified using ‘-to’. Use '-s' to specify a subtitle (smaller text). 
	Example: `/title You are now entering... -s the twilight zone...`

`/raw <"message"> [-suggest|-command <"command"> | -link <"url">] [-hover <"hover message">] [-to <player>] [+ [...]]` Send a raw message. Concatenate with ‘+’. 
	Example:`/raw "Click " + "HERE" -command "hello" -hover "this text is shown only over the HERE" + " to say hello!"` 

`/print <message>` Prints a message that only you can see. 
	Example: `/print &>0+a&m&l&oTEST`

`/do <"command 1"> ["command 2"] ["command 3"]...` Execute multiple commands at once. Do not include a / unless you want to execute //command. 
	Example: `/do "tp @r" "/paste" "kill Akoot_"`

`/homes <player>` List the homes of a player. Click on any coordinates to teleport.

`/home copy <player>` Copy a player's homes (overwrites your own).

`/make <player> say|do <message|command>` Makes a player say/do a message/command.
	Example: `/make Akoot_ say Time to die!` `/make Akoot_ do suicide`

### Navigation

`/!` or `/unstuck` will get you out of a block if you somehow got embedded inside.

`/j` or `/jumpto` sends you to the top of the block that you are looking at. If that block is a vertical wall, you will be placed on top of the cliff at the very edge.

`/thru` sends you through a wall in the direction you are looking.

`/ascend [levels]` and `/descend [levels]` let pass through the ceiling above or floor below you. For example, if you were in a skyscraper on the bottom floor, and used `/ascend 2`, you’d be on the 3rd floor.

`/ceil [clearance]` brings you up to the ceiling of the current room that you are in. If you provide no clearance parameter to use, you will be right up to the ceiling. If you do specify a clearance, the space above your head will be larger. 

`/up <distance>` This will move you up a certain number of blocks.
