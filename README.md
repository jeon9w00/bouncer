# BOUNCER

Minimal mobile arcade game. Draw one line to bounce the ball upward.

## Run locally

Serve this folder with any static HTTP server and open `index.html` (for example, `python3 -m http.server 8765`). No build step is required.

## Progress and cosmetics

The first visit starts a three step tutorial: draw, tilt, bounce again. It continues directly into Infinite. Settings offers a replay option.

Infinite awards one shard every three successful bounces, with additional collectible shards. The Shop in Skins spends these shards on ball and line skins. Ball and line equipment are independent; buying a sports ball also unlocks its matching line. Cosmetic styles do not change physics.

`bounce_world_progress` in local storage keeps the existing World Tour fields and adds `shards`, `unlockedBallSkins`, `unlockedLineSkins`, `equippedBallSkin`, and `equippedLineSkin`. Missing fields are initialized safely for older saves. Tutorial completion uses `bouncer_tutorial_completed`.
