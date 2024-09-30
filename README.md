# One button Spell Rotation Macros for warlocks in World of Warcraft Vanilla

It's a macros group for Spell Rotation for one button, you can use it in raid\groupe, these macros have protection from the wrong target selection.

# Description

Macros group functions;
1) Select a nearby enemy.
2) Check, target status: if the target is in combat.
3) Checking target class(Boss\Mob).
4) Checking the target current HP. If HP is less than 8800hp for mobs, or 40k for bosses, don't cast any debuffs, use just Shadow bolts.
5) Check debuffs on the target and cast Corruption if the target didn't have your Corruption.
6) Cast some Curse, if curse are not on target. If your chosen corruption had on target, casted Curse of Agony
7) If the player has lower mana than 750, and HP is more than 3200, cast Life Tap.

# Requirements

[DoTimer](https://github.com/kc8pnd/DoTimer/) addon needs to check your corruption on target.

[Roid Macros](https://github.com/MarcelineVQ/Roid-Macros/) addon for making group macros, by calling another macro from current, with fixing the length of the macro is more than 250 symbols.

# Instaliation

**Close the World of Warcraft!** before any file changes

Download the file **macros-cache.txt**, and past it to your character folder:
Rename your file **macros-cache.txt** to macros-cache.txt.bak or delete it. This file contains your macros for the character.
```
D:\Games\WoW\WTF\Account\<ACCOUNT NAME>\Nordanaar\<CHAR NAME>
```
Where **\<ACCOUNT NAME\>** is your account name on the server.

Where **\<CHAR NAME\>** is your in-game character name (Your warlock name)

With repository cloning:
# Using PowerShell
```
$characterDir="D:\Games\WoW\WTF\Account\<ACCOUNT NAME>\Nordanaar\<CHAR NAME>"
cd $characterDir
Rename-Item $characterDir\macros-cache.txt -NewName macros-cache.txt.bak
git clone https://github.com/unS0uL/Spell_Rotation_Macros.git
cmd /c mklink "$characterDir" (convert-path ./Spell_Rotation_Macros/macros-cache.txt)
```
