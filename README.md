# LethalRPG – bugs and feedback

This repository holds no code. It is the place for bug reports, compatibility problems and balance feedback for
[LethalRPG](https://thunderstore.io/c/lethal-company/p/Cucumis/LethalRPG/), a personal progression mod for Lethal
Company.

## Before you open an issue

- Read **Known issues & limitations** in the [wiki](https://thunderstore.io/c/lethal-company/p/Cucumis/LethalRPG/wiki/):
  some things are known limits, not bugs.
- Make sure every player in the lobby has LethalRPG in a compatible version: the same minor version, e.g. everyone on
  0.10.x. LethalRPG 0.10.0 uses network protocol 4, so 0.10.x and 0.9.x do not work together: a player with another minor
  version plays without LethalRPG in that lobby.
- Going back to 0.9.0 is possible (below), but then everyone in the lobby has to go back.

## Which form?

| Form | When |
|---|---|
| **Bug report** | Something does not work as described, or LethalRPG breaks the game. |
| **Compatibility** | A problem that only happens together with another mod. |
| **Balance feedback** | An upgrade or skill feels too strong, too weak, too cheap or too slow. |

For a bug, type `rpg report` in the game's terminal right after it happened (or use **WRITE BUG REPORT** in the Rules
tab of the skill menu) and attach the file it writes. It leaves out player names, Steam IDs and your Windows user
folder.

In multiplayer the host first types `rpg selftest` (or clicks **SELF-TEST** in the Rules tab) and waits for the result,
usually within a second: it asks every player's LethalRPG what it holds and applies and compares it with the host's.
The host's report then has the result in its new **SELF-TEST** section. A `MISMATCH` or `WARNING` there is worth
mentioning even when nothing else seems wrong. On a client `rpg selftest` checks only that PC.

For problems with XP, skills, resets, profiles or saves, say where XP and skills are kept: the report's SESSION has the
line `Progress: in profiles` or `Progress: per save (SaveScopedSkills ...)`. Per save is the host's setting
`ProgressScope = Save` (new in 0.10.0, default `Profile`).

## Going back to 0.9.0

If 0.10.0 gives you trouble, you can install LethalRPG 0.9.0 again in your mod manager (r2modman: Installed mods,
LethalRPG, Change version; the menu names differ between mod managers). Everyone in the lobby has to go back, because
0.10.x and 0.9.x do not work together. Profiles keep their format. A save hosted with `ProgressScope = Profile` (the
default) is loaded by 0.9.x. A save played with `ProgressScope = Save` has a new format that 0.9.x leaves untouched, with
a notice that a newer LethalRPG saved it; it is still there when you update to 0.10.x again. More under "Saves and
profiles" in **Known issues & limitations** in the wiki. Please open an issue and say what made you go back.

## Links

- Package page on Thunderstore: <https://thunderstore.io/c/lethal-company/p/Cucumis/LethalRPG/>
- Wiki tab of the package page (host guide, known issues, compatibility, how to report a bug):
  <https://thunderstore.io/c/lethal-company/p/Cucumis/LethalRPG/wiki/>
- The pictures of the package page are in this repository's `media` folder.

## Good to know

- Everything here is public. Do not post Steam profile links, names of other players or paths with your Windows user
  name.
- **Your responsibility:** you decide what you post. The maintainer of LethalRPG is not liable for personal data, Steam
  names, file paths or any other information that you or others publish in issues, comments or attachments. Issues are
  public: others can copy, index or archive them, and deleting something later does not reliably remove it everywhere.
  If you posted something private by mistake, edit or delete it right away.
- Issues are read about once a week. LethalRPG is a hobby project by one person.
- LethalRPG is written with the help of an AI assistant (Thunderstore category "AI Generated").
