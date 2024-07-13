# Scoop FFXIV Bucket
[![Tests](https://github.com/mousseng/scoop-ffxiv/actions/workflows/ci.yml/badge.svg)](https://github.com/mousseng/scoop-ffxiv/actions/workflows/ci.yml) [![Excavator](https://github.com/mousseng/scoop-ffxiv/actions/workflows/excavator.yml/badge.svg)](https://github.com/mousseng/scoop-ffxiv/actions/workflows/excavator.yml)

[Scoop](https://scoop.sh) bucket for software related to FFXIV.

## Quickstart
```pwsh
scoop bucket add ffxiv https://github.com/mousseng/scoop-ffxiv.git
scoop install ffxiv/act ffxiv/act-plugin ffxiv/alexander
```

## Software List
- `act`: [Advanced Combat Tracker](https://advancedcombattracker.com)
- `act-plugin`: the [FFXIV plugin for ACT](https://github.com/ravahn/FFXIV_ACT_Plugin)
- `alexander`: [XIV Alexander](https://github.com/Soreepeong/XivAlexander)
- `fflogs`: the [FFLogs Uploader](https://www.fflogs.com)
- `quicklauncher`: goat's [XIV Quicklauncher](https://github.com/goatcorp/FFXIVQuickLauncher)

## My Personal Setup
I use `quicklauncher` to auto-run `alexander`; to do this, go to the launcher's
`Auto-Launch` settings, press `Add New`, and browse to the scoop install (make
sure you use the `current` path so it continues working through updates). Set
the params to `-a load` so it won't harass you with prompts and enable Kill after
Game Closes.

`quicklauncher` auto-updates, so you don't technically need to use scoop for it.
If you do, you might consider `scoop hold`ing it. Windows is not a fan of symlinks,
so you may find this strategy less problematic.
