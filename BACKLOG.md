# N19 Sunset Static: backlog

Updated 2026-11-19 (v0.2.0). BC decides the order. Plan: `PLAN.md` in this folder. Brief: `BRIEF.md`.

## Done

- 2026-11-19: v0.2.0 Pod and bosses. The pod (front, back, launch, call back, block, touch damage), Spread and Bounce, speed chips, shield cells, the Bass Tower, The Big Disc in three phases, Cruise, Standard and Arcade, five assists, a best score per level. Ship 40 px by default.
- 2026-11-19: v0.1.0 Gray box. Stage 1 from data, auto-scroll, ship, rapid fire, charge beam, five enemy kinds as shapes, shield, beat gates and rewind, settings, 5 slots, Tester tools, start screen, icon, page and Game Shelf card.
- 2026-11-19: day-one setup: `tools/new_game.py` (explore starter, the closest 2D base), kit 1.16.0, Godot 4.7.2, pillars and art style block in `CLAUDE.md`.
- 2026-11-19: reviewed R-Type, wrote the MVP plan, this backlog and the draft brief (G4.8, G4.14).

## Now

- BC's check of v0.2.0. Done when BC beats the boss on Standard and says the pod matters.

## Asked for by BC, not built yet

1. Release 0.3 Look and sound: pixel art, parallax, hit effects, start screen and title track, play music, sound, ten achievements and stats, the title font, the look check and the colorblind check.

## Ideas to choose from (BC picks by number)

1. Stage 2 with a new neon setting: a highway at night, an arcade cabinet world or a city in the rain.
2. Beat sync: enemy waves and bullet patterns timed to the music.
3. More pod shots, such as a ground-hugging shot and a reflect shot.
4. Boss rush mode once there are three bosses.
5. Ship select, each ship with its own charge beam.
6. Score attack per section, personal bests only (G4.4).
7. Photo mode from kit block K10.
8. Local co-op for two players on one screen.

## Later

- Move enemy waves into the kit (K2) once they settle in this game.
- Move the pod into the kit if another game wants a companion that shields and fires.
- A side-scroller genre starter (G10.12) from this game.

## Not planned (they break the pillars)

- Lives, game over or a restart from the start of the stage.
- Losing the pod or pickups on a hit.
- Online leaderboards (G4.4).

## Decisions from BC

- 2026-11-19, 1:36 PM: "a game like R-Type" (N19).
- 2026-11-19, 2:33 PM: "start building a plan for an MVP release for the game in our backlog N19".
- 2026-11-19: soft fail calm level, 2D pixel art, neon synthwave grid, plan kept in `ideas/n19/`.
- 2026-11-19, 2:54 PM: "N19 name picks: N19 name: Sunset Static." From the name decision page.
- 2026-11-19, 3:02 PM: "k2, shooter core next". Kit block K2 comes first.
- 2026-11-19, 3:45 PM: "Sunset Static ship picks: Player ship: B: Needle with bubble canopy." From the ship decision page.
- 2026-11-19, 4:30 PM: "Move the text up more, its bleading into the sun animations". The start screen title sits high, clear of the sun.
- 2026-11-19, 4:32 PM: "Sunset Static title font picks: Title font: Audiowide." From the title font decision page.
- 2026-11-19, 4:35 PM: "Sunset Static pod picks: Pod: 1: Halo Core." From the pod decision page.
- 2026-11-19, 4:35 PM: "ok with the brief". `BRIEF.md` approved (G4.14).
- 2026-11-19, 7:16 PM: "played on my phone, motion is pretty good, seems like the ship should be a little smaller. Lets move to next release". 0.1 feel check passed. Ship set to 40 px. Release 0.2 built.
- 2026-11-19, 6:49 PM: "move to step 2". Release 0.1 built.
- 2026-11-19, 7:05 PM: OK to clone game-signing for the 0.1 APK.
- 2026-11-19, 6:44 PM: "ok, lets go in order starting with 0". N19 starts now, alongside the standards catch-up. Moved from `ideas/n19/` to `games/sunset-static/` through `tools/new_game.py`.
