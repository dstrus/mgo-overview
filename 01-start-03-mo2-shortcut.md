# Mod Organizer 2

Hey, kids! It's your Uncle Davey!

So you have Mad God's Overhaul downloaded and installed.

Now you can manage the installed list and launch the game via Mod Organizer 2.

Here I have a nearly-pristine installation of MGO SFW 3.8.8.1. I’ve only added a couple of mods that I know will be included in the next release and which will make this video look quite a bit better.

Personally, I play several mod lists for a couple different games that all use Mod Organizer 2 (which, for the sake of brevity, I’ll call “MO2” from now on). Now you can pin each copy of MO2 to the Taskbar or Start Menu, but they’ll all have the same icon, and they’ll all be labeled `Mod Organizer`. This isn’t a “how to use Windows” tutorial, but frankly they’ve made this sort of customization such a pain recently that I’ll show you how I’ve done it. Remember, you can always skip ahead.

## Pinning a shortcut to Mod Organizer

Find your MGO installation folder in File Explorer, and find `ModOrganizer.exe`. (By the way, you can open File Explorer any time with `Win` + `E`. It's my favorite keyboard shortcut in all of Windows.) Right-click the icon and drag it just a bit, within the same folder, and choose `Create a shortcut` from the context menu. You can name the shortcut whatever you want, like `Skyrim VR MGO`. You can also change the icon. Right-click, Properties, Change Icon. If nothing else, you can set it to Skyrim’s icon. I think the Skyrim VR icon is ugly, so how about the Skyrim SE icon? Or a custom icon for MGO!

Having done that, I'll right-click one of the shortcuts that's already pinned to my Start Menu and choose `Show Original`. You might expect this to show the _original_ original, but it actually shows the pinned shortcut. It's weird. It also happens to be convenient for what we're trying to achieve. Drag your MGO shortcut from the MGO installation folder into the same location as the other pinned shortcuts, right-click the shortcut, and pin it to the Start Menu. _Et voilà_!


## Launching Mod Organizer

Once you launch it, MO2 takes a little while to start. Even the splash screen doesn't show up right away. Resist the temptation to launch it again. Just wait.


## Before you play...

When MO2 has finished loading, you can launch the actual game with the `▶️ Run` button near the upper-right, with `Play Game (SKSE)` selected in the nearby dropdown. You should always launch MGO this way. Don't just run Skyrim VR from Steam. That will just launch vanilla. Launch the game from MO2 if you want to play MGO.

But first, let's have a look around.

Frankly, there's a lot going on here. If you don't care to know more, you can skip ahead. You don't absolutely need to know more about MO2. But I won't be going into excruciating detail about MO2's innards. I'll just give you the highlights. So consider sticking around a little longer.


## Interface overview

MO2's interface is basically split in two.

The left pane is the mod list. Aside from some separators that are there for the sake of organization and documentation, each row in the left pane is a mods. Most of them are packaged mods that you can download from Nexusmods or somewhere similar. Others are specific to MGO.

Mods can be groups under collapsible separators. You can expand each group by clicking the arrow to the left of each separator. Each mod, then, will have a checkbox to its left. If the box is checked, that mod is enabled. If it's unchecked, the mod is disabled, and will not be included when you run the game.

Many, but not all, of the mods listed in the left pane have corresponding plugins on the right.

The right pane will probably show the `Downloads` tab the first time you run MO2, but there's much much to say about that. Switch to the `Plugins` tab. It's more interesting.

There are three types of files listed in the `Plugins` tab: `.esm` files, `.esp` files, an `.esl` files.

### Masters (`.esm`)

Those with the `.esm` extension are Elder Scrolls Masters. This format dates back to Morrowind. These are the base game files, including the official DLCs. Some of the big DLC-sized overhaul mods, like Vigilant, use the master format too.

Masters always load before regular plugins. They also count towards the limited number of slots in Skyrim's load order.


### Regular Plugins (`.esp`)

The files with an `.esp` extension are Elder Scrolls Plugins. This format also dates back to Morrowind. This is the "normal" format for the things that mods can contain aside from loose files. Plugins can contain things like quests, behavior, object placement. Stuff like that. These also count towards Skyrim's load order limit.


### Light Plugins (`.esl` and ESL-flagged `.esp`)

Light plugins are new to Skyrim Special Edition. All of the light plugins together share a single slot in the load order, so they make huge mod lists like MGO far more practical. There is still a limit to how many light plugins you can use, but it's a lot.

Light plugins have their own file extension (`.esl`), but some of them still have the `.esp` extension. Those have been ESL-flagged, so they behave like `.esl` plugins, despite their file extension.

So why aren't all plugins ESL-flagged? Well, there's a limit to how many new records a light plugin can contain. Light plugins also can't add a new worldspace. So some plugins have to remain full-blown ESPs, and they count towards the lower limit.

MGO was designed around the limit, of course, so you don't have to worry about it unless you start adding to the list yourself... which I'm sure you will. I'm not going to do a deep dive into that right now though. As susceptible as I am to scope creep, even I have my limits. 

There are other tools in this dropdown that you may need on occasion if you start fiddling with the mod list, but we’re not there yet. Also, you can create a shortcut that actually launches the game instead of launching MO2. If you’d rather pin that to the Start Menu or Taskbar, you know how.
