First, you'll want to head over to `https://ultravanilla.world`.
At the bottom right, you should see this window here, and you're gonna want to click the "Login" button as shown.

![](https://i.imgur.com/WNlBU9c.png)

From there you're gonna see a window pop up telling you about your "Account". In order to login, do as the site says and run the command `/token` in-game.

![](https://i.imgur.com/QLAfRMy.png)

When you do that command it should give you a link and this message.

![](https://i.imgur.com/1kxkcCZ.png)

If you click the link, it should take you to a webpage that will have this:

![](https://i.imgur.com/5j5JBGW.png)

Feel free to select for however long you want to stay logged in for. Use your own judgement for how secure your computer is etc, please note that in the future we will have a lot more sensitive information on the staff section of this site.

Once that's done, it should take you back to the main site, and you can see that the "Login" button has changed to your role and name.

![](https://i.imgur.com/gNrstYb.png)

If you click on it, it should open up a window telling you that you're logged in, and it should show links to all the staff tools we have available. Currently, the only staff tool is one that helps with coreprotect.
Click on it and follow along to learn how it works.

![](https://i.imgur.com/iLiUyHs.png)

When you enter this site, you're gonna notice it's a bit scary! Do not worry, you do not need to write or read a  single line of code. Bear with me and do as I say and you'll notice it's actually a lot easier than it looks.

![](https://i.imgur.com/TkOFAwk.png)

There are 3 text boxes, each  one with a different purpose. You do not need to edit the 1st box or the 3rd box. The only box you will be putting information inside of is the 2nd box, hence the "Compute" button below it.

What goes on the 3rd box is actually your minecraft logs, which may take some work to find. Before we find that though, let's prepare your log for this tool to work correctly.

The purpose of this tool is that sometimes thieves know that admins can lookup transactions and try to hide their tracks by creating pages and pages of transactions, making it very difficult to look up. Gone are the days of writing down every single transaction and performing calculations by hand! Just follow the steps below and you should be golden.

Before you inspect the chest, be sure to run `/lag` (no reason why, lordpipe just chose that)
After that, run `/co i`, and then right click a chest.
Do as many page lookups as you like using `/co l <page>`, don't worry if people chat or if you do other commands in-between, just make sure to only inspect that chest until you have enough info.

Sometimes people take up pages and pages of lookup data to hide their tracks, so I've created something that might help.
Here's a command that you can paste to run 10 pages of lookup for you (every 1.5 seconds).
If you onlt need like 5 pages and not 10, please remove the remaining `co l #`'s from the command as it will be redundant.
`/do delay:1.5 "co l 1" "co l 2" "co l 3" "co l 4" "co l 5" "co l 6" "co l 7" "co l 8" "co l 9" "co l 10"`

Once you've looked up all the pages, you can copy your log to the site.
Your `latest.log` file is where minecraft stores all chat, debug, and information logs for the game. It is usually located in `%appdata%\.minecraft\logs`, and `%appdata%` is usually `C:\Users\<Your Username>\AppData\Roaming` on Windows. If you're on mac it will be under `~/Library/Application Support/minecraft/logs` (Look up "Minecraft folder mac" if you can't find it).
But, if you're on windows, and you don't use any fancy launchers or profiles, feel free to press CTRL+R and type this in: `notepad %appdata%\.minecraft\logs\latest.log`. It will open up your `latest.log` without having to look for it.

Feel free to select everything (CTRL+A) and paste it to the 2nd box on the site.
If you want, you can search for the section in your `latest.log` that contains the data you want to lookup, but it's not necesarry. And if you did `/lag` before you looked things up, everything above it will be ignored.

After you're done, go ahead and click on "Compute delta", and something should pop up on the last text area.
All of this may seem scary and weird if you haven't seen it before but it's quite simple really.
The only section you should be worried about is the `"delta"` section. For me, it looks like this in this instance.
```json
"delta": {
        "Dusk_95": {
            "torch": 3
        },
        "kekhon": {
            "cooked_chicken": 4
        },
        "Freak_Genius": {
            "diorite": 6
        },
        "YodaSmiling": {
            "cooked_chicken": 1,
            "cooked_porkchop": 1,
            "firework_rocket": 14
        },
        "iElijah": {
            "iron_chestplate": -1,
            "iron_leggings": -1,
            "iron_boots": -1,
            "iron_ingot": -4,
            "iron_helmet": -1
        }
    },
```
This might make it a little easier to understand:
```yml
Dusk_95:
- Added 3 torches
kekhon:
- Added 4 cooked chicken
Freak_Genius:
- Added 6 diorite
YodaSmiling:
- Added 1 cooked chicken
- Added 1 cooked porkchop
- Added 14 firework rockets
iElijah:
- Took 1 iron chestplace
- Took 1 iron leggings
- Took 1 iron boots
- Took 4 iron ingots
- Took 1 iron helmet
```
And that's it! Now you know exactly how much is taken and put in the chest no matter how many pages the lookup takes.
Easier to use version to come!
