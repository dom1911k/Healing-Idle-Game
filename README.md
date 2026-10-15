# Mendwright

A small healing game in a single HTML file. It mixes the party healing and spell-focused skill tree of **Master Healer Kale** and **Mini Healer** with Cookie Clicker–style idle income and an **Astlibra**-style item mastery system.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press its number. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Dungeons.** Eight dungeons, each 5–10 stages of monster packs ending in a boss. Health and mana carry over between stages, with a short rest. Every dungeon has a rule of its own (poison, a silenced spell, scorching air, weaker healing, low mana, an early berserk timer). Each new dungeon is much harder than the last, so you farm until you're ready, then choose to push on.
- **You lose** if you die or the rest of the party dies. Rewards from stages you cleared are kept. With *Repeat dungeon* on, the run starts again by itself.

## Spells and skills

- You start with only **Heal**. Bosses drop **Rubies** (always on a first clear, sometimes after that), which teach new spells: Flash Heal, Renew, Ward, Purify, Meditate, Prayer, Sanctuary and Blessing.
- Every spell has its own branch in the **Skills** tab, plus a Cleric branch of passives. Skill points come from Cleric levels and first dungeon clears. Refunds are free.

## Other progression

- **Levels.** Every cleared stage gives experience to all five heroes. Each level adds 7% health and damage.
- **Gear.** Enemies drop items for six slots in five rarities. Enchant equipped items with gold for +10% stats per level.
- **Item mastery.** Every item teaches a skill. Clear stages with it equipped to master it, and the skill is yours for good.
- **The sanctum.** Healing earns gold. Buildings earn gold every second, blessings are one-time upgrades, and the Barracks trains party damage, health and regeneration. Buildings keep earning for up to 8 hours while you're away.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, +1 Ruby, win the current stage, unlock the next dungeon, drop an item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
