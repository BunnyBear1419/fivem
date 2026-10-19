# FiveM local timecycle troubleshooting

## Important: do not install the archived `cielo.xml.xmas-backup`

That file contains only one timecycle named `XMAS`; it is not a clean, general-purpose replacement for the normal FiveM/GTA V timecycle data. It is preserved only as a backup for inspection.

## Reversible local test to remove the unwanted Christmas/snow override

1. Fully close FiveM.
2. Open `%LOCALAPPDATA%\\FiveM\\FiveM.app\\citizen\\common\\data\\timecycle` in File Explorer.
3. If `cielo.xml` is present, copy it somewhere safe as `cielo.xml.backup` first.
4. Rename the local `cielo.xml` to `cielo.xml.disabled` (do not delete it yet).
5. Start FiveM and test a server where the roads/grass/sidewalks looked snowy.
6. If the issue remains, rename it back and investigate the graphics pack's streamed textures/timecycle files next. This test isolates the local override; it does not guarantee all snow textures are caused by this file.

Keep ReShade and your graphics pack installed during this test. Do not edit `timecycle_mods_1.xml`, `timecycle_mods_2.xml`, or `timecycle_mods_3.xml` as part of this first isolation step.
