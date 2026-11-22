# N19 Sunset Static: backlog

Updated 2026-11-22 (v0.10.0). MVP plan complete. Two stages, no bosses, coins and a shop, HD painted backgrounds, HD ship and pod. BC decides the order. Plan: `PLAN.md` in this folder. Brief: `BRIEF.md`.

## Done

- 2026-11-22: v0.10.0 HD painted ship and pod (BC: "we need a hd graphic for the ship, it looks lo resolution compared to the background now", then picked "HD paint, brighter neon" for the ship and "HD paint" for the pod). `tools/make_hd_sprites.py`. Hitboxes unchanged.
- 2026-11-22: v0.9.0 HD painted backgrounds (BC: "add higher quality images for the background", then picked HD paint for Stage 1, Stage 2 and the start screen and "Live neon lines, upgraded" for the floors). Gemini layers through the art workflow (G8.8), cut by `tools/make_hd_bg.py`. Per stage tints. Kit 1.27.0, full screen by default in the browser, 120 frames a second, vibrate permission.
- 2026-11-19: v0.8.0 Coins and the shop. Every enemy drops coins by size. A shop after each stage (and in the Menu) sells permanent Ship, Pod, Helper and Look upgrades. Neon arrow charge beam (BC's pick). Beat gates as small diamonds. Wide screens filled edge to edge (G6.21).
- 2026-11-19: v0.7.0 New enemies, no bosses. BC: no boss battles. The Bass Tower, The Big Disc and The High Score are gone: each stage ends with a final wave section. Four new enemies made with Gemini and Meshy: the Strobe Pair and Ring Carrier in Stage 1, the Prize Claw and Bumper Bot in Stage 2.
- 2026-11-19: v0.6.0 Stage 2 finished (idea 1, part 2). The High Score boss (Paddle Ball, Snake and Block Drop on its screen), Stage 2 music Bit Quest (BC's pick), music and tempo per stage, Stage 2 colorblind check.
- 2026-11-19: v0.5.0 Stage 2 "Insert Coin" (idea 1, part 1). The arcade cabinet world, Blips, coin bugs, coins, the checkered floor, Stage 2 opens after The Big Disc, Menu stage rows.
- 2026-11-19: v0.4.0 Smoother flying and beat sync (idea 2). Ease in and out, smoothed drags, screen-pixel drawing, steadier tilt. Waves, enemy shots and bosses on the beat of the play music. Grid pulse locked to the music.
- 2026-11-19: v0.3.0 Look and sound. Pixel art drawn in code, three parallax layers, bursts and sparks, the beat pulse, BC's music picks (Drama, Neon Laser Horizon), Kenney sounds, look check, colorblind check and name check. The MVP plan is done.
- 2026-11-19: v0.2.0 Pod and bosses. The pod (front, back, launch, call back, block, touch damage), Spread and Bounce, speed chips, shield cells, the Bass Tower, The Big Disc in three phases, Cruise, Standard and Arcade, five assists, a best score per level. Ship 40 px by default.
- 2026-11-19: v0.1.0 Gray box. Stage 1 from data, auto-scroll, ship, rapid fire, charge beam, five enemy kinds as shapes, shield, beat gates and rewind, settings, 5 slots, Tester tools, start screen, icon, page and Game Shelf card.
- 2026-11-19: day-one setup: `tools/new_game.py` (explore starter, the closest 2D base), kit 1.16.0, Godot 4.7.2, pillars and art style block in `CLAUDE.md`.
- 2026-11-19: reviewed R-Type, wrote the MVP plan, this backlog and the draft brief (G4.8, G4.14).

## Now

- BC's check of v0.10.0: the HD ship and pod, plus the 0.9 paintings, readability, the floor pulse, the start screen and 120 frames a second on his phone.
- Playtest sweep results (BC, 2026-11-19, 8:59 PM): good: Stage 2 Insert Coin and the upright view on his phone.
- MVP done (BC, 2026-11-19, 8:11 PM: "it was fun to play throuhg").
- Next: BC picks from the ideas below, or Stage 3 (a highway at night or a city in the rain).

## Asked for by BC, not built yet

- Nothing open. Stage 2 (idea 1) is done.

## Ideas to choose from (BC picks by number)

10. HD paint for the enemies, coins, pickups and shots, so everything matches the HD ship and backgrounds (the pixel enemies stand out next to them now). Same route: Gemini paintings of the approved designs, picked on a decision page.
3. More pod shots, such as a ground-hugging shot and a reflect shot.
9. Remake the eight code-drawn enemies (drifter, mini, turret, charger, splitter, shell, Blip, coin bug) with Gemini and Meshy, like the 0.7 enemies (BC, 2026-11-19: keep them for now).
5. Ship select, each ship with its own charge beam.
6. Score attack per section, personal bests only (G4.4).
7. Photo mode from kit block K10.
8. Local co-op for two players on one screen.

## Later

- Kit pieces off in this game since the 1.27.0 pull (K rule 3), each needs BC's yes: phone fit (`touch_min_dp`), the safe area, the Android back swipe, the title focus guard, `glow2d.gd` halos, `fx2d.gd` particles, `haptics.gd` buzz styles (the game calls no buzz yet, so Rumble does nothing on the phone), `score.gd` (K12, G4.17 rollout), `tester_notes.gd` (T1), `ShooterCore.Waves` (K2) and the easy pack (K8).
- Lossy WebP import for the HD backgrounds if the web build size (56 MB) or phone memory becomes a problem.
- The start screen redraws its painting every frame even with Reduce motion on. A small saving at 120 frames a second.
- A test that checks the Reduce flashing setting reaches the start screen (today only the play floors and calm are tested).
- Slow the pod's spin or drop its cyan beat arc now the pod is HD, if it reads busy in play.
- An HD painted Stage 3 when BC picks it, made the same way (sky, far row, near row on a green screen).
- Move enemy waves into the kit (K2) once they settle in this game.
- Move the pod into the kit if another game wants a companion that shields and fires.
- A side-scroller genre starter (G10.12) from this game.
- Stage 3 in one of the other settings: a highway at night or a city in the rain.
- A kit helper for the music position (the game reads the kit's player today).

## Not planned (they break the pillars)

- Boss battles (BC, 2026-11-19: "I dont want boss battles though, just enemies in each level"). The 0.2 to 0.6 bosses were removed in 0.7. Boss rush mode (old idea 4) is dropped.
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
- 2026-11-19, 8:25 PM: "Sunset Static Stage 2 picks: Stage 2 setting: Arcade cabinet world." From the Stage 2 decision page.
- 2026-11-19: "Finish Stage 2 (0.6)". The High Score boss, Stage 2 music and checks.
- 2026-11-19, 8:45 PM: "Sunset Static Stage 2 music pick: Stage 2 play music: Bit Quest (Kevin MacLeod)." From the Stage 2 music decision page.
- 2026-11-19, 9:03 PM: "move on to adding new enemies using the gemini meshy workflow. I dont want boss battles though,, just enemies in each level". Picks: remove all three bosses, two new enemies per stage, keep the code-drawn enemies, designs on a decision page.
- 2026-11-19, 9:38 PM: "Sunset Static enemy picks: Strobe Pair (Stage 1, Grid Run): B: Crystal lens. Ring Carrier (Stage 1, Grid Run): A: Cargo hauler. Prize Claw (Stage 2, Insert Coin): B: Boxy grabber. Bumper Bot (Stage 2, Insert Coin): C: Saucer bumper."
- 2026-11-19, 9:57 PM: "you can always download files that you need to and dont need to ask".
- 2026-11-19, 10:19 PM: "the enemies need to drop coins so i can buy upgrades at the end of each level". Picks: Ship, Pod, Helpers and Looks upgrades, permanent, coins from every enemy by size, the shop after each stage clear.
- 2026-11-19, 10:20 PM: "why is there a yellow bar down the middle of the screen... i dont like it, change that". The beat gate line became two small diamonds at the screen edges.
- 2026-11-19, 10:27 PM: "Sunset Static beam pick: Charge beam look: Neon arrow." From the charge beam decision page.
- 2026-11-19, 10:35 PM: "seems like the game is 4:3 and not 16:9, the effects the background dont go th full width", then "all games need to support 1080p 16:9 screens". Scenery now fills wide screens. New standard G6.21.
- 2026-11-19, 8:21 PM: "move forward".
- 2026-11-19, 8:13 PM: "continue with your suggestions, it would be nice to improve the moviement of the ship to be smooother". Beat sync and smoother flying in 0.4.0, then Stage 2.
- 2026-11-19, 8:11 PM: "it was fun to play throuhg, what is next in the backlog". MVP signed off.
- 2026-11-19, 8:02 PM: "Sunset Static music picks: Start screen title track: Drama (Holizna). Play music: Neon Laser Horizon (Kevin MacLeod)." From the music decision page.
- 2026-11-19, 7:50 PM: "move on to the next release". Picked art drawn in code and a music decision page now. Release 0.3 built.
- 2026-11-19, 7:16 PM: "played on my phone, motion is pretty good, seems like the ship should be a little smaller. Lets move to next release". 0.1 feel check passed. Ship set to 40 px. Release 0.2 built.
- 2026-11-19, 6:49 PM: "move to step 2". Release 0.1 built.
- 2026-11-19, 7:05 PM: OK to clone game-signing for the 0.1 APK.
- 2026-11-19, 6:44 PM: "ok, lets go in order starting with 0". N19 starts now, alongside the standards catch-up. Moved from `ideas/n19/` to `games/sunset-static/` through `tools/new_game.py`.
