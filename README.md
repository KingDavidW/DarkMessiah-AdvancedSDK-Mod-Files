# Dark Messiah Advanced SDK Module Files
The mod files for the DM Advanced SDK Base. This is the final set of files, not compliable code. Most mods will need this 

## Dependencies
wiltOS Dark Messiah Mod Launcher [Download](https://www.moddb.com/games/dark-messiah-of-might-magic/downloads)

## How to Install
Make sure you have the wiltOS Dark Messiah Mod Launcher installed!

Go to the **_mods** folder in your Dark Messiah game, and create a new folder titled **advanced_sdk**

Take the files from this repository and extract them into that folder.

## Mod Order Requirement
Make the Advanced SDK the first mod in your list, above everything else. That ensure all the hooks are bound correctly!

## Opt-in compatibility for one tested non-Steam 1.02 build
The launcher repository's [compatibility contribution](https://github.com/KingDavidW/DarkMessiah-ModLauncher-Files/pull/8)
provides a single source-only Python patcher for both the launcher and this SDK.
It supports only the exact game/module SHA-256 profile documented there; it
does not claim support for every non-Steam or Steam version.

For SDK R2-03.23 (`c5a6fb8f84bf9e6bc4f463b45655d812d1d59e15`), the supported
`server_sdk.dll` input SHA-256 is
`CEC5327A05F7A461BA34784D267877797301AB844C91F5A927A73AAD68290B9D`.
The patcher changes operand RVAs `0x19BDC9` and `0x19BE81`, producing
`344F54B392458F97DF5FFE4F372027F17D9C36CC41877578B849287BE5FF7621`.
Its complete game-version guards, byte checks, installation instructions,
transactional backups/rollback and tests are maintained in the launcher
contribution, rather than duplicated here. This documentation does not replace
the distributed DLL or change the standard Steam installation.

## Recommended Installation
The best way to install this mod is by actually doing a git checkout to that **advanced_sdk** folder. That way, as this mod updates, you can just download the changes instead of redownloading the whole repository. I recommend [Github Desktop](https://desktop.github.com/download/) to make it easier, but it is entirely up to you.

## Credits
King David for doing the programming and bug fixing

Valve for the initial SDK
