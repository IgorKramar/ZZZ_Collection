<div align="center">

# ZZZ Industrial Collection

**English** · [Русский](README.ru.md)

### A working homestead in a fallen Kentucky.

Project Zomboid Build 42 · Steam Workshop mods · A ready-to-use starter kit

![Project Zomboid](https://img.shields.io/badge/Project_Zomboid-Build_42-e0af68?style=flat-square)
![Format](https://img.shields.io/badge/starter_kit-ZIP-9ece6a?style=flat-square)
![Load order](https://img.shields.io/badge/load_order-Mod_Load_Order_Sorter-bb9af7?style=flat-square)
[![Steam](https://img.shields.io/badge/Steam-Workshop-7aa2f7?style=flat-square)](https://steamcommunity.com/sharedfiles/filedetails/?id=3778214259)

[Install](#install) · [Starter kit](#starter-kit) · [Flagship mods](#flagship-mods) · [Compatibility](#compatibility) · [Support](#support) · [Rights](#credits-and-rights)

</div>

![ZZZ Industrial Collection — modpack banner](banner.jpg)

**Light the forge, assemble the machines, plough the field, fix the truck.**
ZZZ is an industrial survival modpack for Project Zomboid **Build 42.20.2+**. This repository supplies the configuration that a Workshop subscription does not install: the enabled-mods list and load-order rules, plus setup guides in English and Russian.

The bundled starter kit targets **100 enabled mods** and was documented as tested on **42.20.2**. Workshop mods and newer game builds can change independently; the kit is not a guarantee that every current combination has been retested.

## Install

1. In Steam, open **Project Zomboid → Properties → Betas** and select the `b42` branch described by the starter kit.
2. Open the [Workshop collection](https://steamcommunity.com/sharedfiles/filedetails/?id=3778214259), choose **Subscribe to all**, and wait for all downloads to finish (several GB).
3. Download [`ZZZ_Collection_StarterKit.zip`](ZZZ_Collection_StarterKit.zip). **Close the game and back up your existing `default.txt` and `sorting_rules.txt` before copying:** the supplied files replace your current enabled-mods list and load-order rules.
4. Copy `Zomboid/mods/default.txt` from the archive to `C:\Users\<name>\Zomboid\mods\`, and `Zomboid/Lua/sorting_rules.txt` to `C:\Users\<name>\Zomboid\Lua\`.
5. Launch the game. On the mods screen, press **Sort and accept**, provided by **Mod Load Order Sorter**.

These are Windows profile paths. For another operating system or a custom profile, use its actual `Zomboid` directory. To enable mods manually instead, follow `README_INSTALL_EN.txt` inside the archive, including its exclusions below.

## Starter kit

| Archive entry | Purpose |
|:---|:---|
| `README_INSTALL_EN.txt` | Full installation and setup guide in English |
| `README_УСТАНОВКА.txt` | Full installation and setup guide in Russian |
| `Zomboid/Lua/sorting_rules.txt` | Rules consumed by Mod Load Order Sorter |
| `Zomboid/mods/default.txt` | Ready-made enabled-mods list |

**The archive contains configuration and documentation, not the Workshop mods.** Steam downloads those separately. No build toolchain is required to use this kit.

## Flagship mods

| Mod | Role |
|:---|:---|
| [Hydrocraft Reinvented [B42]](https://steamcommunity.com/sharedfiles/filedetails/?id=3778201332) | Thousands of items and recipes ported to B42's native `craftRecipe` system |
| [ZZZ Mod Stitch [B42]](https://steamcommunity.com/sharedfiles/filedetails/?id=3778211804) | Compatibility patches and a startup validator for the collection |
| [ZZZ RusPack [B42]](https://steamcommunity.com/sharedfiles/filedetails/?id=3778212091) | Additional Russian translations for mods with missing or incomplete localization |

Russian localization follows the game's language setting when ZZZ RusPack is enabled. Individual mods supply their own other languages.

## Compatibility

<details>
<summary><strong>Do not enable these entries</strong></summary>

- **Capacity Limit Bypass [MANUAL INSTALLATION]** asks for manual game-engine file replacement. The starter kit explicitly excludes it; do not install it as part of this pack.
- **Somewhat Traits Skills** duplicates functionality provided by **Legendary Professions and Traits**. It is disabled in the supplied list.

</details>

<details>
<summary><strong>Map priorities and expected warnings</strong></summary>

Use **Map Mod Manager** to choose the winning map where cells overlap:

| Maps | Cells |
|:---|:---|
| Constown / New Hartburg | `24_42`–`24_44` |
| Louisville Quarantine Zone / PIE42 | `44_13`, `45_13` |

The bundled guide identifies yellow warnings about these overlaps and `tiledef 7001` (Customizable Containers / Fort Waterfront) as known conditions. Other red validator messages should be reported rather than ignored.

</details>

<details>
<summary><strong>First launch and Horse Mod</strong></summary>

After enabling Horse Mod, fully restart the game before playing. The kit warns that enabling it without a restart can leave animation placeholders instead of horses.

</details>

Keep the full guides in the ZIP nearby: they describe the configuration shipped here. Updates to the game or Workshop collection may require adjustments.

## Support

Post in the relevant mod's Workshop discussions or the [collection comments](https://steamcommunity.com/sharedfiles/filedetails/?id=3778214259). Include the game version, affected mod, single-player/server context and the relevant tail of your profile's `console.txt`.

## Credits and rights

Collection assembled and maintained by **hombrehumor**. The included Workshop mods belong to their respective authors; their distribution and reuse terms remain separate.

This repository currently contains no `LICENSE` granting blanket reuse rights for the collection or starter kit. A download link does not relicense third-party mods, artwork or game resources. Check the relevant authors' terms before redistributing their material.
