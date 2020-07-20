## Minecraft 1.16 is out! 
Besides the nether and a lot of neat things they have added RGB COLOR! So I've been working hard on making that possible for us country folk.
First things first, for custom colors the only format accepted by the server will be in **hexadecimal**. If you don't know what that is I recommend you use [this site](https://www.w3schools.com/colors/colors_picker.asp "this site") or look up "color picker" on google or something.

Your color should be in this format:`#000000` and the 0's can be any number or letter from `0-9` and `a-f`. Capitalization is ignored.

---

## Here's how you do color text in game:

#### Single Colors

`&#ff0000TEST` will result in a red TEST, and so on. Just think of it like using color codes such as &a but instead of 'a' just replace it with a custom color. Must contain the # or it won't work.

#### Gradients
`&>#ff0000+#00ff00TEST` will the text "TEST" have a gradient from left to right from this color`#ff0000`to this color`#00ff00`.

_If you want to use color codes instead you may, as well as color names such as `dark_green` and `aqua`. You can also mix and match such as:`&>red+#0000ff`and`&>c+3`and`&>gold+4` etc. Here's a guide for [color codes](https://www.digminecraft.com/lists/color_list_pc.php "color codes") if you want to use those too._

## Applying this to /namecolor

**_Note: The syntax for`/namecolor`has changed slightly. There's 3 different ways to use this command._**

#### Single color
`/namecolor color` This can be any one color such as `red` or `#ff0000`. 
	Example: `/namecolor red`or`/namecolor #66d9ff `

#### Gradient
`/namecolor color1+color2` Just put a `+` between 2 colors to give your name a gradient.
	Example: `/namecolor #c299ff+black`or`/namecolor red+white`

## Two-color
`/namecolor color1+color2 na+me` The first part is selecting 2 colors combining them with a `+` then the second part is specifying where in your name you want to make the split.
	Example: `/namecolor green+yellow no+tch`or`/namecolor #b3b300+#5c5cd6 jeb+_` the `+` symbol stating that everything to the left of it will be the first color and everything to the right of it will be the second color. 

**_Note: The second argument MUST match your username or current nickname (without color) otherwise you must use /nick if you have permission._**

## Applying this to /nick
 You may use the syntax described above (Example: `/nick &#FF0000Santa` `/nick &>6+4Fireball`), but if you simply want a 2-color name, a gradient (if you have permission), or even just a 1-color name, I recommend using `/namecolor` instead (`/nc` for short).
