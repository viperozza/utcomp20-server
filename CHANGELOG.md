# Changelog

## [2.1.0] - 2026-11-27

- Added a custom Lightning Gun zoom scope.
- Added an energy shield with hit effects to the Shield Gun alt-fire.
- Added options to toggle the new shield and Lightning Gun visuals
  independently.
- Added a scoreboard flag choice and nickname gradient presets.
- Enabled the server footstep audio fix by default (`bEnableFootstepFix`; set
  it to `False` in `UTCompv20.ini` to restore the previous behavior).

## [2.0.5c] - 2026-11-19

- Fixed ladder rank lookups never completing on hosts that do not close the
  connection after the reply (such as Windows dedicated servers); the rank
  badges now apply as soon as the full response has arrived.

## [2.0.5b] - 2026-11-19

- Fixed a server crash caused by a stale weapon fire reference kept by the
  sustained-fire rewind (Minigun and Link Gun hit registration).
- Fixed ladder rank badges not appearing on UTDuel servers running DuelGame
  with more than two player slots.
- Added state-change logging for rank lookups to make rank service problems
  easier to diagnose.

## [2.0.5] - 2026-11-19

- Fixed Minigun and Link Gun hit registration during sustained fire.
- Added the new Shield Belt (100 armor) mesh with a refreshed skin.
- Added scoreboard nickname fonts, with preview and Apply in Colored Names, and
  showed each player's chosen font on the Deathmatch scoreboard.
- Added ladder rank badges (Bronze to Legend) on Duel and TDM scoreboards,
  tiered by the global Duel and TDM ELO, plus a Ranks menu page listing every
  badge and its ELO range.

## [2.0.4] - 2026-10-28

- Added a pulsing hot-orange Assault Rifle grenade treatment with a brighter
  trail and dynamic glow.
- Improved Shield Gun reflection coverage for frontal shots striking the
  collision cylinder's flanks, lower legs, and shoulders.
- Restored the original K4 Shock primary correction behavior while retaining
  UTComp v20 miss statistics and diagnostic logging.
- Added the October 2026 changes to the scrollable in-game development log.

## [2.0.3] - 2026-09-18

- Refreshed scoreboard layout and behavior, including the top-player highlight.
- Added new Shock combo visuals, a hitsounds-everywhere option, smoother
  eye-height behavior, and an expanded in-game development log.

## [2.0.2] - 2026-09-04

- Refined the Damage Taken recap with clearer hit, headshot, damage, and share
  columns.
- Recorded Sniper headshots as a dedicated subset of incoming Sniper hits.

## [2.0.1] - 2026-09-04

- Added the Damage Taken scoreboard recap.

[2.1.0]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.1.0
[2.0.5c]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.0.5c
[2.0.5b]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.0.5b
[2.0.5]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.0.5
[2.0.4]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.0.4
[2.0.3]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.0.3
[2.0.2]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.0.2
[2.0.1]: https://github.com/viperozza/utcomp20-server/releases/tag/v2.0.1
