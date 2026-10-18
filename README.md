# DBM-Whitemane

Deadly Boss Mods for the **Whitemane Frostmourne** realm, the 3.3.5a (Wrath of the Lich King) server that launched in **September 2026**.

Frostmourne doesn't run the encounters exactly as Blizzard shipped them. Bosses have custom mechanics, changed ability timers and re-tuned numbers, so a stock 3.3.5 DBM shows timers that drift, misses abilities and warns for things that no longer happen. This build is adjusted to how the fights actually play on Frostmourne:

- **Custom mechanics.** Warnings, special announces and voice callouts for abilities Frostmourne added or changed.
- **Timers.** Ability, phase-change and enrage timers re-measured against the live encounters.
- **Tunings.** Health thresholds, phase transitions, stack counts and range checks match Frostmourne's numbers.

It is built on the 3.3.5a DBM backport by Zidras and the DBM-Frostmourne contributors (DBM-Core 11.5.5).

## Installation

1. **Remove any other DBM first.** Delete every `DBM-*` folder from `World of Warcraft\Interface\AddOns\`. Mixing two DBM versions causes errors and duplicate warnings.
2. Download the zip from **Releases** (or **Code → Download ZIP**).
3. Copy **all** the `DBM-*` folders from the zip into `Interface\AddOns\`.
   If you used *Download ZIP*, copy the folders *inside* `DBM-Whitemane-main`, not that folder itself.
4. Restart the game.

Open the options with `/dbm`.

## What's included

| Folder | What it is |
|---|---|
| `DBM-Core` | The engine: warnings, timers, sounds, range check, info frame, arrow, boss health |
| `DBM-GUI` | The options window (`/dbm`) |
| `DBM-StatusBarTimers` | The timer bars |
| `DBM-SpellTimers` | Optional bars for long raid cooldowns |
| `DBM-Range2` | A second, independent range radar (`/range2`) |
| `DBM-VPVEM` | English voice pack ("VEM", female voice) for spoken callouts |
| `DBM-Icecrown`, `DBM-Ulduar`, `DBM-Coliseum`, `DBM-Naxx`, `DBM-ChamberOfAspects`, `DBM-EyeOfEternity`, `DBM-Onyxia`, `DBM-VoA` | Wrath raids |
| `DBM-Karazhan`, `DBM-BlackTemple`, `DBM-Sunwell` | Burning Crusade raids |
| `DBM-MC`, `DBM-ZG` | Classic raids |
| `DBM-Party-WotLK`, `DBM-Party-BC`, `DBM-Party-Classic` | Dungeons |
| `DBM-PvP`, `DBM-WorldEvents` | Battlegrounds and holiday bosses |

The raid and dungeon modules only load when you enter that zone. To keep things lighter, you can leave out:
- the modules for content you don't run
- `DBM-VPVEM`, if you don't use voice callouts

## Notes

- Report wrong timers or missing warnings with the boss name, the difficulty (10/25, normal/heroic), and what happened versus what DBM showed. A screenshot of the timer bars helps.
- This build is for Frostmourne. On other 3.3.5a realms its timers won't match.
