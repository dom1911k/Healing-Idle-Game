# Mendwright

A small healing game in a single HTML file. It mixes the party healing of **Master Healer Kale**, a Path of Exile–style talent web, and **Mini Healer** with Cookie Clicker–style idle income and an **Astlibra**-style item mastery system.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press its number. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Dungeons.** Eight dungeons, each 5–10 stages of monster packs ending in a boss. Health and mana carry over between stages, with a short rest. Every dungeon has a rule of its own (poison, a silenced spell, scorching air, weaker healing, low mana, an early berserk timer). Each new dungeon is much harder than the last, so you farm until you're ready, then choose to push on.
- **You lose** if you die or the rest of the party dies. Rewards from stages you cleared are kept. With *Repeat dungeon* on, the run starts again by itself.

## The talent tree

- You start with only **Heal**. Every other spell (Flash Heal, Renew, Ward, Purify, Meditate, Prayer, Sanctuary, Blessing) is a node in the talent tree.
- The tree is a web, in the style of Path of Exile, that spreads outward from the centre through six schools: **Mending** (Heal and Flash Heal), **Growth** (Renew), **Protection** (Ward, Sanctuary and the tank), **Devotion** (mana and Meditate), **Command** (party damage, gold, experience and Blessing) and **Purity** (critical heals, haste, Purify and Prayer). An inner and an outer ring link neighbouring schools.
- You can take any talent next to one you already have. Small talents cost 1 point, notables 2, spells 3–4, and keystones 3. Keystones are big trade-offs such as *Martyr's Vow* (healing +25%, max mana −20%).
- Talent points come from Cleric levels (1 each) and first dungeon clears (2 each). You can refund any talent nothing else depends on, or refund everything for free.
- Drag to pan, scroll or use the buttons to zoom, click a talent to see it, and double-click to allocate.

## Other progression

- **Levels.** Every cleared stage gives experience to all five heroes. Each level adds 7% health and damage.
- **Gear.** Enemies drop items for six slots in five rarities. Enchant equipped items with gold for +10% stats per level.
- **Item mastery.** Every item teaches a skill. Clear stages with it equipped to master it, and the skill is yours for good.
- **The sanctum.** Healing earns gold. Buildings earn gold every second, blessings are one-time upgrades, and the Barracks trains party damage, health and regeneration. Buildings keep earning for up to 8 hours while you're away.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, +5 talent points, win the current stage, unlock the next dungeon, drop an item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
