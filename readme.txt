[b]Explorer Tools Version 1.2[/b]
This mod adds a pick, axe, and shovel that not only dig on a left click, but will place whatever item is in the inventory slot immediately to their right on a right click.

Have you ever been frustrated when digging a mine or exploring a cavern because you have to dig, dig, dig, then swap the active inventory item to a torch, place a torch, swap the active inventory item back to your pick, and repeat?  Did you ever wish that you could just place a torch (or a block of stone or glass) with a right click while still wielding your pick, axe, or shovel?  If so, then this mod is for you!

The tools are based upon the diamond versions, and are crafted by replacing the top stick in the recipe with a mese crystal:
[code]
diamond,   diamond   ,diamond        diamond,diamond              diamond
       ,mese fragment,               diamond,mese fragment      mese fragment
       ,   stick     ,                      ,stick                 stick
[/code]
[img]http://i57.tinypic.com/2maaog.png[/img]

These tools have the same stats as a diamond tool, with the exception that the uses has been increased by 10%.  (to account for the extra expense of adding a mese crystal)
The tools work exactly like the base diamond version, EXCEPT that when wielding these tools, if you right click, it does a "place" using the item directly to the right in the players inventory.  So, for example, if your inventory slots looked like this:

[img]http://i60.tinypic.com/11huw7k.png[/img]

Then a left click with the pick would dig, but point the pick at the wall and right click, and it will place a torch from your second inventory slot on the wall.  No need to switch active inventory items at all.  Left click to dig with the pick, right click to place a torch.

And it doesn't have to be a torch.  Perhaps you are building a project that requires digging out stone and replacing it with glass.  Just put your stack of glass in the inventory slot next to the explorer pick, dig the stone out with a left click, place the glass with a right click.  The axe and the shovel work the same way.

[b]Alternative mod:[/b]
There was a request that the explorertool place on rightclick function be added to every pick, axe, and shovel in the game.  4aiman implemented this in his magichet game, and kindly gave me permission to create an explorertoolsall mod based on his code.  Download THAT version if you want ALL tools to be able to place an item on right click.

[b]Possible future changes:[/b]
The textures, eh, not so great here.  If someone gets inspired to suggest an improvement, I'm very open to it.  I didn't create an explorer hoe, because there was not a diamond version of the hoe in the default game, but adding a hoe would be simple.
This is my first MineTest mod, and my first time ever programming in Lua, so any suggestions for improvements in the code are very welcome.

[b]Credits:[/b]
My son helped me with the idea, the programming, and the textures.  Thanks to kaeza for sample code of how to get the inventory item to the right of the tool, and to PilzAdam and Stu for answering my questions about how the uses field works.  4aiman for the change the code for Explorer Tools All.

[b]Incompatibilities:[/b]
Do not use with Inventory Tweak mod, on right click your tool will disappear!

[b]---For Explorer Tools:[/b] (use this one for special explorer tools)
[b]Dependencies:[/b]
soft depends on default, but without default you have no recipe.

[b]License:[/b] CC0

[b]To browse source:[/b]
[url]https://github.com/Kilarin/ExplorerTools[/url]

[b]Download:[/b]
[url]https://github.com/Kilarin/ExplorerTools/archive/master.zip[/url]

[b]---For Explorer Tools All:[/b] (use this one to let all tools do a right click place)
[b]Dependencies:[/b]
Soft depends on default.  Add soft dependencies for any other tool mods you want this to affect.

[b]License:[/b] gplv3

[b]To browse source:[/b]
[url]https://github.com/Kilarin/explorertoolsall[/url]

[b]Download:[/b]
[url]https://github.com/Kilarin/explorertoolsall/archive/master.zip[/url]

[b]---[/b]

[b]To install:[/b]
Simply unzip the file into your mods folder, and rename the folder to explorertools (Or explorertoolsall)
OR, simply install it directly from minetest using the online mod repository.

[b]Mod Database:[/b]
If you use either of these mods, please consider reviewing it on the MineTest Mod Database.
[url]https://forum.minetest.net/mmdb/mod/explorertools/[/url]
[url]https://forum.minetest.net/mmdb/mod/explorertoolsall/[/url]

[b]Change Log:[/b]
1.2 change from kaeza: Force-update stack instead of relying on success indicator.
    This eliminates a problem where using explorertoolsall and an itemframe would
    allow you to duplicate items.  And, to my surprise, it does not seem to cause
    you to lose items when you can't place the stack.
1.1 changed hard depends on default to soft
    removed requirement that index pos of tool be less than 8
    updated readme to include explorertoolsall referenc
1.0 initial release