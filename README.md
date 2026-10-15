# Mendwright

A small healing game in a single HTML file. It mixes the boss-by-boss party healing of **Mini Healer** and **Master Healer Kale** with Cookie Clicker–style idle income and an **Astlibra**-style power curve built from many stacking sources.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press `1`–`5`. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Spells:** Mend (slow, efficient), Flash Heal (fast, costly), Renew (heal over time, stage 2), Ward (absorb shield, stage 4), Prayer (heals everyone, stage 6).
- **Bosses** auto-attack the tank and cast telegraphed abilities (Cleave, Searing Wave, Shadow Bolt, Festering Bite, Frenzy). They enrage below 20% health and go berserk after 2 minutes.
- **You lose** if you die or the rest of the party dies. Beat the boss to unlock the next stage, or step back to farm.

## Where power comes from

- **Levels.** Every victory gives experience to all five heroes (half for the fallen). Each level adds 6% health and damage. Your Cleric's levels also raise healing and mana and grant talent points.
- **Talents.** Three branches (Light, Devotion, Command) with 15 talents. Deeper talents need points spent in their branch. Refunds are free.
- **Gear.** Bosses drop items for six slots in five rarities, with stats like Spell Power, Max Mana, Mana Regen, Critical, Haste, Gold Find and Party Vigor. Enchant equipped items with gold for +10% stats per level.
- **Item mastery.** Every item teaches a skill. Win fights with it equipped to master it, and the skill is yours for good, even after you sell the item. Ranks stack from different items up to V.
- **The Libra.** Offer items to the Light pan (healing) or the Shadow pan (party damage and health). The bonus grows with each pan's total karma, but only while the scales are within 10% of level. Perfect balance adds 10% to everything.
- **The sanctum.** Healing earns gold (overhealing doesn't). Buildings earn gold every second, and each one costs 15% more than the last. Blessings are one-time upgrades. The Barracks trains party damage, health and regeneration.
- **Offline earnings.** Buildings keep earning while you're away, for up to 8 hours.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, win fight, skip 5 stages, drop item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
