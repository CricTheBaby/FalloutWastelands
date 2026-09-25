<div align="center">

# FALLOUT: WASTELANDS

### A Passion Project

</div>

Fallout: Wastelands is a free, fan-made multiplayer version of Fallout 3 and Fallout: New Vegas. It is built from scratch in the Godot Engine and reads the worlds, characters, quests and items straight from **your own** copies of the games, so you can explore the Capital Wasteland with friends: quests, V.A.T.S., the Pip-Boy, parties, clans, player homes and a shared world that keeps moving while you're in a menu.

It is a hobby project made by fans, and it is still in active development. Expect rough edges, and please tell us about them (see [Reporting bugs](#reporting-bugs)).

---

## Legal notice

- Fallout: Wastelands is a **non-profit fan project**. It is free, and it will never be sold or monetised.
- It is **not affiliated with, endorsed by or sponsored by** Bethesda Softworks, ZeniMax Media or Microsoft. Fallout, Fallout 3, Fallout: New Vegas and related names and logos are trademarks of their respective owners.
- To play you need **legally owned** copies of **Fallout 3: Game of the Year Edition** (with all five add-ons) and **Fallout: New Vegas**, installed on your PC.
- **No game files are distributed here.** Nothing from Bethesda's games (models, textures, sounds, maps, music, text) is in this repository or in any download. The game reads them from your own installs, on your own PC, when you play.
- **No mod files are distributed here either.** The optional mods listed below stay on their authors' own pages. The launcher only helps you download them from Nexus Mods with your own account.

See [LICENSE_NOTICE.md](LICENSE_NOTICE.md) for what our license covers and what it doesn't.

---

## Requirements

| | |
|---|---|
| **Operating system** | Windows 10 or Windows 11, 64-bit |
| **Fallout 3** | Fallout 3: Game of the Year Edition, with all five add-ons (Operation Anchorage, The Pitt, Broken Steel, Point Lookout, Mothership Zeta), installed |
| **Fallout: New Vegas** | Installed (Steam or GOG) |
| **Disk space** | About 300 MB for Fallout: Wastelands itself, plus about **10 GB free** for the game data it prepares from your installs on the first start (you can choose which drive this goes on) |
| **Graphics card** | A card that supports **Vulkan** (most NVIDIA, AMD and Intel cards from the last ~8 years). Keep your graphics drivers up to date. |
| **Internet** | Needed to install, update, download mods and play online. Single player still starts when you're offline. |

**Graphics settings.** In the launcher (OPTIONS) and in the game (Settings > Graphics) there is a **Quality Preset**:

- **LOW** looks like the original game and is the lightest. Try this first on older or laptop graphics chips.
- **MEDIUM** adds ambient occlusion, bloom and god rays, and costs only a little more than LOW.
- **HIGH** (the default) adds screen-space lighting and reflections. Aimed at mid-range cards.
- **ULTRA** adds soft shadows, full global illumination and volumetric fog. For fast cards.

The game has been developed and tested on an NVIDIA RTX 4060 Ti at 1080p. If your frame rate is low, drop the preset one step, or turn on FSR upscaling in Settings > Graphics.

---

## How to install

1. **Download** the latest `Fallout Wastelands Setup.exe` from the [Releases page](https://github.com/CricTheBaby/FalloutWastelands/releases/latest) (under **Assets**). There is also a `.zip` of the same thing if your browser or file host doesn't like `.exe` files.
2. **Run it.** Windows may show "Windows protected your PC". Click **More info**, then **Run anyway** (see the [FAQ](#faq) for why).
3. **Pick the install folder.** The default (`%LOCALAPPDATA%\Fallout Wastelands`) is fine. The installer makes desktop and Start menu shortcuts and opens the launcher.
4. **The launcher finds your games.** It looks in Steam, GOG, the Windows registry and the usual folders. The status panel shows FALLOUT 3 and NEW VEGAS as FOUND. If one says NOT FOUND, open **GAME FOLDERS** and use **BROWSE** to point it at the game's folder.
5. **Get the mods (optional).** The **MODS** page opens by itself the first time. Press **LOG IN WITH NEXUS MODS** and the launcher fetches the mods for you (see [Mods used](#mods-used)).
6. **Press PLAY.** The first start prepares the game data from your installs, with a progress bar. This takes a few minutes and only happens once.

---

## Mods used

Fallout: Wastelands can use these community mods if they are in your Fallout 3 / New Vegas `Data` folders. **All of them are optional today.** The game has a fallback for each one and plays fine without any of them.

| Mod | Author | Nexus page | Needed? | What it's used for |
|---|---|---|---|---|
| Enhanced Movement | TBD | [New Vegas mod 85459](https://www.nexusmods.com/newvegas/mods/85459) | Optional | Prone crawling animations and the long sprint stride. Without it, prone uses the crouch poses and sprint uses the normal run. |
| Enhanced Animations | TBD | [New Vegas mod 95967](https://www.nexusmods.com/newvegas/mods/95967) | Optional | Smoother walking, running and weapon animations. Without it, the original animations are used. |
| New Vegas True Scopes | TBD | [New Vegas mod 74824](https://www.nexusmods.com/newvegas/mods/74824) | Optional | See-through 3D rifle scopes with the mod's reticles and per-weapon zoom. Without it, the game's own scope view is used. |
| NMC's Texture Pack (Fallout 3 and New Vegas versions) | NMC | TBD ([search](https://www.nexusmods.com/newvegas/search/?gsearch=NMC%27s+Texture+Pack)) | Optional | Sharper world and armour textures. Install each version into its own game's `Data` folder. |
| Fallout Character Overhaul (FCO) | TBD | TBD ([search](https://www.nexusmods.com/newvegas/search/?gsearch=Fallout+Character+Overhaul)) | Optional | Better faces, eyes and hair textures. |
| Project Beauty | TBD | TBD ([search](https://www.nexusmods.com/fallout3/search/?gsearch=Project+Beauty)) | Optional | HD face and body textures for Fallout 3's people. |
| Weapon Retexture Project (WRP) | TBD | TBD ([search](https://www.nexusmods.com/newvegas/search/?gsearch=Weapon+Retexture+Project)) | Optional | Sharper New Vegas weapon models and textures (used by the New Vegas weapon models option). |

**We never host mod files.** Mods belong to their authors, and many contain Bethesda material, so they are only ever downloaded from the author's own Nexus Mods page, with your own Nexus account:

- **Nexus Premium:** the launcher downloads and installs missing mods automatically in the background.
- **Free Nexus account:** Nexus only allows downloads started on its website. The launcher's **DOWNLOAD** button opens the mod's Files page; click **Mod Manager Download** there and the launcher takes it from there. One click per mod. (The launcher asks once to handle Nexus download links. If you use Vortex or Mod Organizer it tells you and lets you choose.)
- **Logging in:** until our single sign-on is approved by Nexus, the login button opens your Nexus **API keys** page. Copy your **Personal API Key**, paste it into the launcher and press **SAVE KEY**. It is stored only on your PC, is only ever sent to Nexus Mods, and **LOG OUT** deletes it.

Any game file a mod replaces is backed up first, and the launcher remembers every file it installed so updates and removal are clean. Mods with an installer that asks questions (FOMOD) need to be installed with a mod manager or by hand. You can of course install any of these mods yourself instead. The launcher detects them either way.

---

## Updating

Updates are automatic. Every time the launcher starts it checks this repository for a new release, downloads only the files that changed, checks them, and swaps them in. If anything goes wrong it puts the old files back, so you are never left with a half-installed game. PLAY is greyed out until the update is done.

- Your settings, saves, characters and folder choices are never touched by an update.
- If you are offline, the launcher says it couldn't check, and you can still play single player with the version you have.
- The launcher's **NEWS** page shows the notes for the version you have installed. Every release's notes are also on the [Releases page](https://github.com/CricTheBaby/FalloutWastelands/releases).
- When a new release lists a new mod, the MODS page marks it **NEW**.

---

## Community

Come and say hello, find people to play with, and follow development on our Discord:

**https://discord.gg/rpSwBw9Rt4**

The launcher's NEWS page has a **JOIN THE DISCORD** button too. Update notes, server status and the live bounty board are posted there.

---

## Reporting bugs

Please report bugs in the **#bug-reports** forum on the [Discord](https://discord.gg/rpSwBw9Rt4). One post per bug helps a lot. Useful things to include:

- what you were doing, and what happened versus what you expected
- a screenshot or short clip, if you can
- your version (shown in the launcher's status panel, VERSION row)
- whether you were in single player, hosting, or on a server
- your graphics card and the Quality Preset you use
- for crashes: the log files from `%APPDATA%\Godot\app_userdata\Wasteland\logs\`

---

## Credits

- **Bethesda Game Studios** and **Obsidian Entertainment**, for Fallout 3 and Fallout: New Vegas, the games this whole project is a love letter to. Please buy them: you need them to play.
- **The mod authors** whose work Fallout: Wastelands can use: the authors of Enhanced Movement, Enhanced Animations, New Vegas True Scopes, NMC's Texture Pack, Fallout Character Overhaul, Project Beauty and the Weapon Retexture Project (see [Mods used](#mods-used)). Please endorse their mods on Nexus Mods.
- **The [Godot Engine](https://godotengine.org)** and its contributors. Fallout: Wastelands runs on Godot 4, which is free and open source (MIT license).
- **The Fallout modding community**, whose decades of documentation on the games' file formats made a project like this possible.
- Everyone on the Discord who plays, tests and reports bugs.

---

## FAQ

**Does it work with the Steam or GOG versions of the games?**
Yes. The launcher looks for both Steam and GOG installs, including Steam libraries on other drives. For Fallout 3 you need the Game of the Year Edition (or the base game with all five add-ons installed). Other store versions should work too, as long as the game files are installed on your PC. If the launcher doesn't find them, see the next question.

**The launcher can't find my game.**
Open **GAME FOLDERS** in the launcher. Next to Fallout 3 or New Vegas, press **RESCAN** to search again, or **BROWSE** and pick the game's folder (the one that contains `Fallout3.exe` / `FalloutNV.exe` and the `Data` folder). Make sure the game has been installed and started at least once through Steam or GOG.

**My antivirus or Windows SmartScreen warns about the download.**
Fallout: Wastelands isn't signed with a paid company certificate, and brand-new files from small projects often get flagged because few people have downloaded them yet. That is a false positive. Only download from this repository's [Releases page](https://github.com/CricTheBaby/FalloutWastelands/releases). To run it: SmartScreen > **More info** > **Run anyway**. If your antivirus quarantines the file, you can restore it and add the install folder as an exception. If you're unsure, ask on the Discord.

**Where are my saves?**
Single-player saves are in `%APPDATA%\Godot\app_userdata\Wasteland\saves\` (paste that into the File Explorer address bar). Settings are in the same `Wasteland` folder. You can move the saves folder in the launcher's **GAME FOLDERS** page. Multiplayer characters are saved on the server you play on.

**Where does the ~10 GB of game data go? Can I move it?**
By default it's `%APPDATA%\Godot\app_userdata\Wasteland\fo3_cache`. It is prepared from your own game installs and never leaves your PC. In **GAME FOLDERS** you can move it to another drive (the launcher copies it with a progress bar).

**Do I need the mods?**
No. Every mod is optional right now, and the game plays without any of them. They make things look and move better.

**Do I need Nexus Premium?**
No. A free account works: you click **Mod Manager Download** once per mod. Premium just makes it fully automatic.

**Does it change my Fallout 3 or New Vegas install?**
Only if you install mods through the launcher. It copies the mod's files into the game's `Data` folder, like any mod manager, after backing up any file it replaces. The game itself only reads your installs.

**Is it free?**
Yes, and it always will be. If anyone is selling it, it isn't us.
