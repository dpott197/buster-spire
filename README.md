# Quiver Spire

A TowerFall-style archery arena that runs in the browser. Fight AI archers solo, or host an online room and send friends a link.

**Play:** https://dpott197.github.io/quiver-spire/

## Scoring

Every KO scores a point, by arrow or by landing on someone's head. KO'd archers respawn after two seconds, flickering for a moment while they can't be hit. Hitting yourself with your own arrow costs a point. First to the KO target (5, 10 or 20) wins the match.

## Online play

1. Click **Host online**. You get a link like `https://dpott197.github.io/quiver-spire/#K7QX5`.
2. Send it to up to three friends. They open it, pick a name and join.
3. Click **Start match**. AI archers fill any empty seats, and take over if someone leaves.

The host's browser runs the match and friends connect to it directly over WebRTC ([PeerJS](https://peerjs.com/) handles the connection setup). There is no game server. The host should keep the page open for the whole match. A few strict networks block direct connections; if a friend can't join, try another network.

## Controls

| Action | Keys |
| --- | --- |
| Run | ← → or A D |
| Aim up / down, drop through ledges | ↑ ↓ or W S |
| Jump (wall-jump against walls) | Z, J or Space |
| Shoot (8 directions) | X or K |
| Dodge (catches arrows) | C, L or Shift |
| Pause (host only online) | Esc or P |

Phones get on-screen buttons.

The whole game is `index.html`, with no build step.
