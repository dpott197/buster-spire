# Buster Spire

A robot arena shooter that runs in the browser, inspired by classic run-and-gun games. Charge your arm cannon, slide under shots, and battle AI robots or friends online.

**Play:** https://dpott197.github.io/buster-spire/

Forked from [Quiver Spire](https://github.com/dpott197/quiver-spire), the TowerFall-style version. Not affiliated with or endorsed by Capcom; all names and art are original.

## How it plays

- Every robot has **three energy**. A small shot takes one, a half charge takes two, a full charge takes all three. Landing on a robot's head takes all three.
- **Tap** to fire small shots, up to three on screen at once. **Hold** the shoot button to charge, then let go: the robot flashes blue at half charge and white-gold at full charge. A full charge shot pierces through robots.
- After a hit, a robot is knocked back and flashes for a moment, during which it can't be hurt.
- **Slide** along the ground to duck under shots. In mid-air, the same button dashes sideways.
- Double-jump in mid-air, wall-jump off walls, and drop down through grates.
- Your own shots can't hurt you.

## Modes

Every mode is played in rounds. A round lasts until one robot (or one team) is left, or 90 seconds pass.

| Mode | How you score |
| --- | --- |
| **Head Hunters** (default) | 1 point per KO. First to the KO target wins. |
| **Last Man Standing** | 1 point for being the last robot running in a round. |
| **Team Head Hunters** | Red against Blue. Every KO scores for your team. Teammates can't hurt each other. |

## Weapon capsules

Capsules drop into the arena during each round. Touch one to open it. Special shots fire before your buster and don't charge. Everything resets at the end of the round.

| Capsule | Effect |
| --- | --- |
| Bomb shot | Three lobbed bombs that explode on impact |
| Ricochet laser | Three fast beams that bounce off walls |
| Shock field | Two shots that leave a crackling field rivals can't touch |
| Drill shot | Three shots that bore through one block |
| Barrier | Blocks the next hit completely |
| Jet boots | Boost as often as you like in mid-air |
| Turbo boots | Run faster |
| Energy tank | Refills your energy |

## Online play

1. Click **Host online**, or type a code in **Room code** first to get the same link every time (for example `#MONSIEUR`).
2. Send the link to up to three friends. They open it, pick a name and join.
3. Click **Start match**. AI robots fill any empty seats, and take over if someone leaves.

The host's browser runs the match and friends connect to it directly over WebRTC ([PeerJS](https://peerjs.com/) handles the connection setup). Rooms are separate from Quiver Spire's, so the same code can be used in both games.

## Controls

| Action | Keys | Controller |
| --- | --- | --- |
| Run | ← → or A D | Stick or d-pad |
| Aim up / down, drop through grates | ↑ ↓ or W S | Stick or d-pad |
| Jump, double-jump, wall-jump | Z, J or Space | A |
| Shoot (hold to charge) | X or K | X or Y |
| Slide / air dash | C, L or Shift | B, bumpers or triggers |
| Pause (host only online) | Esc or P | Start |

Phones get on-screen buttons.

The whole game is `index.html`, with no build step.
