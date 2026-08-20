# Talhalla

**▶ Play it in your browser: https://qwendor.github.io/talhalla/**

A Brawlhalla-inspired 2D platform fighter, built from scratch in a single HTML file.
No dependencies, no build step — just open `index.html` in any browser
(or run `powershell -File serve.ps1` and visit http://localhost:4173).

## Fighters

Pick your fighter on the character select screen (move with left/right, confirm
with your light-attack button, unconfirm with heavy, ESC to go back). In 1-player
mode the bot picks a random character.

| | BLOCKY | NYX | TOR | SAGE | REX |
|---|---|---|---|---|---|
| Style | Balanced all-rounder | Speedy ninja | Hammer brute | Long-range mage | Lance knight |
| Speed | ●●○ | ●●● | ●○○ | ●●○ | ●●○ |
| Power | ●●○ | ●○○ | ●●● | ●●○ | ●●● |
| Weight (launch resistance) | ●●○ | ●○○ | ●●● | ●○○ | ●●○ |
| Air jumps | 2 | 3 | 1 | 2 | 2 |
| Signature | Reliable sword arcs | Near-instant daggers, huge dash-slash | Slow, massive hammer swings | Wide arcane blasts from far away | Long thin pokes that KO sideways |
| Recovery (↑ + heavy in air) | Rising Uppercut — big vertical boost with a hit | Shadow Step — teleport up-forward with i-frames | Skyfall Vault — huge armored leap with a hit | Arcane Lift — floaty rise with an AoE hit | Pole Vault — diagonal launch with a lance hit |

Each fighter gets ONE recovery per airtime; it refreshes when you land.

Four more fighters round out the roster of 9 (plus a secret 10th):

| | VOLT | GLACIA | FANG | WREN |
|---|---|---|---|---|
| Style | Storm spirit | Ice queen | Werewolf rushdown | Archer |
| Gimmick | Lightning strikes with tall hitboxes that launch enemies UPWARD — KOs off the top | Slowest runner but the highest jumps, and the strongest spike in the game | Tiny claw range but huge damage; every attack lunges him forward | Heavy attacks fire REAL arrows that arc, stick into stages, and skewer story enemies — the only true ranged fighter |
| Recovery | Sky Bolt — the biggest vertical boost, with a zap | Glacier Rise — floaty AoE lift | Pounce — a steep diagonal leap with a bite | Wind Ride — an upward gust vault |

Beat the story campaign to unlock **THE DEVOURER** himself as the 10th fighter.

## Supers

Taking damage fills the meter under your fighter. When it's full, press
**light + heavy together** to unleash your character's super — a cinematic
screen-freeze followed by a signature haymaker (BLOCKY's HEROIC NOVA blast,
NYX's THOUSAND STARS blink-shred, WREN's SKYFALL VOLLEY arrow rain, TOR's
WORLDBREAKER eruption, and so on — every fighter has their own).

## Maps

After both players lock in, pick one of six themed battlefields:

- **SKYHOLM** — the classic: main stage + three soft platforms, under twinkling stars.
- **TWIN PILLARS** — two towers with a deadly gap, drifting embers in a sunset sky.
- **GREAT HALL** — one wide flat floor, fireflies in the gloom. Pure footsies.
- **MAGMA KEEP** — obsidian isles over a glowing lava sea with rising sparks.
- **FROSTPEAK** — an asymmetric frozen summit in constant snowfall.
- **NEON ROOFTOPS** — three rain-slick rooftops over a lit-up cyberpunk skyline.

## Items

Toggle with **T** on the main menu or map select (saved between sessions; in
online games the host's setting applies). When on, an item crate parachutes
in every 15 seconds (max 2 waiting). Walk into it to grab it — it floats over
your head — then press your **light attack to throw it** (hold up/down to
angle the throw):

- **💣 Bomb** — arcs through the air and explodes on contact or after a short
  fuse: 18 damage and big radial knockback to everyone in range.
- **🪃 Boomerang** — flies out, then homes back to you; hits on the way out
  AND the way back, and you can catch it for a re-throw.
- **🏐 Bouncy ball** — ricochets off the stage with heavy bounces, clobbering
  anyone it touches (even you, after the first moments) until it burns out.

## Dash-dodge

Dodge now *dashes*: press dodge while holding any direction (including diagonals
and straight up) to burst that way with invincibility frames. Neutral dodge
(no direction) still works as a stationary i-frame dodge. Up-dash is a handy
extra recovery tool; down-dash dives. Same 18 i-frames, same cooldown.

## Game modes

- **CLASSIC** — the standard duel: vs Bot or 2 players on one keyboard/gamepads. Pick fighters, pick a map, 3 stocks each.
- **PARTY** — 2-4 player free-for-all on one keyboard (and/or up to 4 gamepads). P1 is in; P2/P3/P4 press any of their controls to join on the character select, then everyone picks a fighter and a map. Last one with a stock left wins.
- **ONLINE** — 2-4 players over the internet (WebRTC peer-to-peer, no server or accounts needed — just internet). One player picks **HOST A ROOM** and shares the 5-character room code; the others pick **JOIN WITH CODE** and type it in. Everyone picks a fighter in the shared lobby and readies up (A/D to pick, F to ready), the host chooses the map, and the free-for-all begins. Every player uses their own machine's **P1 controls** (WASD + F/G/H, or gamepad 1). The host's game runs the match; if the host closes the game, the room ends. After a match the host presses ENTER to bring everyone back to the lobby for a rematch.
- **ARCADE** — a 5-stage gauntlet. Pick your fighter, then defeat every champion in the biome that represents them: BLOCKY at Skyholm, NYX at Neon Rooftops, TOR at Magma Keep, SAGE at Great Hall, REX at Twin Pillars. Lose once and the run is over.
- **SURVIVAL** — pick a fighter and a map, then bots spawn in endlessly (up to 3 at once, waves speed up over time, each bot has 1 stock). Every bot you beat = 1 point. Your best score is saved between sessions and shown on the menu.
- **STORY — The Devourer Saga** — 1-4 player co-op campaign, playable locally **or online**: in an online lobby the host presses W/S to switch the mode from VERSUS to any unlocked STORY chapter, and the whole room plays it together. Beating the final boss **unlocks THE DEVOURER as a playable fighter** (he fights as his own face). 1-4 player local co-op campaign. Four side-scrolling chapters to explore (the camera follows your team through levels wider than the screen), packed with unique enemies: **Shades** (melee stalkers), **Wisps** (flying chasers), **Spikers** (turrets that shoot), and **Brutes** (horned tanks) — all with health bars you grind down; no friendly fire. Fall in a pit and you respawn next to a living teammate. Reach the swirling portal to clear a chapter (progress saves; chapters unlock one by one). Chapter 5 is the throne room of **THE DEVOURER** — a boss with a huge HP bar, ground-slam shockwaves, aimed fireballs, a charge attack, and minion summons; at half health it enrages. Wipe and you can retry the chapter instantly.

## How it plays

- Damage stacks up as you get hit (the circle in the HUD goes white → red).
- The more damage you have, the farther attacks send you flying.
- Get launched past the edge of the screen and you lose a stock. 3 stocks each — last fighter standing wins.
- Modes: **1 Player (vs Bot)** or **2 Players** on one keyboard.

## Controls

Keyboard and gamepads both work (and can be mixed). The first connected
controller drives Player 1, the second drives Player 2.

| Action | Player 1 (kbd) | Player 2 (kbd) | Gamepad |
|---|---|---|---|
| Move | A / D | ← / → | Left stick / D-pad |
| Jump (double jump in air) | W | ↑ | A |
| Fast-fall / drop through platform | S | ↓ | Stick down / D-pad ↓ |
| Light attack | F | , | X |
| Heavy attack | G | . | Y or B |
| Dodge (invincible) | H | / | LB / RB / triggers |
| Spike (in air) | S + G | ↓ + . | Stick ↓ + Y |
| Menus | W/S + Enter | — | D-pad + A / Start |

Players 3 & 4 (Party mode) — keyboard, or gamepads 3 and 4:

| Action | Player 3 | Player 4 |
|---|---|---|
| Move | I J K L | Numpad 8 4 5 6 |
| Light attack | O | Numpad 7 |
| Heavy attack | P | Numpad 9 |
| Dodge | [ | Numpad 0 |

Gamepad buttons use the standard layout (Xbox naming above; on PlayStation
A/X/Y/B correspond to Cross/Square/Triangle/Circle).

## Mechanics

- **Knockback scaling** — `knockback = base + damage × scale`, so kills come from racking up damage first.
- **Hitstun, hitstop and screen shake** on every hit; heavies freeze the frame longer.
- **Dodge** gives 18 frames of invincibility with a 70-frame cooldown.
- **Soft platforms** can be dropped through with Down; the main stage is solid.
- **Spike** (down + heavy in the air) sends airborne opponents straight down.
- Respawn comes with brief invincibility (flicker) and resets your damage.
