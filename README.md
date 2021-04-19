# neoreset

_Neo's auto resetter for Minecraft speedrunning on Linux._

---

## TL;DR

Download the latest release from here:

- **[neoreset 1.0.0 (Linux)](https://github.com/younishd/neoreset/releases)**

Run the executable (e.g. from a terminal) and press…
- **F7** to reset (from title screen)
- **F8** to switch category

## Features

- **RSG/SSG/FSG**
- Global and per session counter in world name
- Included filters
    - filteredseed
    - filteredvillage
    - filteredshipwreck
    - ruined-portal-loot
    - fsg-power-village-looting-sword

## Settings

Check out the file called `neoreset.json` in your `.minecraft` folder.

- `hotkey` - reset hotkey
- `hotkey2` - switch category hotkey
- `delay` - delay in seconds between simulated keyboard inputs
- `session_thresh` - threshold when to wrap a session (in seconds)
- `sound` - voice on/off
- `world_name` - world name format string with placeholders
    - `{c}` - category
    - `{v}` - version
    - `{s}` - per session counter
    - `{g}` - global counter
- `ssg.seed` - seed to be used for SSG category
- `fsg.filter` - filter to be used for FSG category
    - `filteredseed`
    - `filteredvillage`
    - `filteredshipwreck`
    - `ruined-portal-loot`
    - `fsg-power-village-looting-sword`

## Work in progress

- [x] 1.16
- [ ] 1.14
- [x] RSG
- [x] SSG
- [x] FSG
- [x] Linux
- [ ] macOS
- [ ] Windows

(PRs are welcome.)

## Dev

```
git clone https://github.com/younishd/neoreset.git
cd neoreset
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
./neoreset.py
```

## Bugs

Feel free to report any issues [here](https://github.com/younishd/neoreset/issues) or DM me (`neo#0495`) on discord.

## Credits

Thanks to [@AndyNovo](https://github.com/andynovo) for the FSG goodies.
