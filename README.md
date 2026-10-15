# Mendwright

A small healing game in a single HTML file. It mixes the party healing of **Master Healer Kale**, WoW-style talent trees, and **Mini Healer** with Cookie Clicker–style idle income and an **Astlibra**-style item mastery system.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press its number. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Dungeons.** Eight dungeons, each 5–10 stages of monster packs ending in a boss. Health and mana carry over between stages, with a short rest. Every dungeon has a rule of its own (poison, a silenced spell, scorching air, weaker healing, low mana, an early berserk timer). Each new dungeon is much harder than the last, so you farm until you're ready, then choose to push on.
- **You lose** if you die or the rest of the party dies. Rewards from stages you cleared are kept. With *Repeat dungeon* on, the run starts again by itself.

## Cleric talents

- You start with only **Heal**. The other eight spells are learned in the talent trees.
- Three WoW-style trees: **Holy** (Heal, Flash Heal, Prayer), **Discipline** (Ward, Purify, Sanctuary, the tank) and **Devotion** (mana, Renew, Meditate, Blessing).
- Most talents take 5–10 ranks of small bonuses. Ranks 1–5 cost 1 point and later ranks cost 2. Major talents (2–3 points) and new spells (3–4 points) sit between them.
- Deeper rows need points spent in that tree first: 2 per row.
- Talent points are rare: 1 every 2 Cleric levels, plus 1 for each first dungeon clear. Resetting is free.

## The party

- Companions attack on their own timers. Every hit has its own damage, attack speed, critical chance and critical damage. Melee hits land at the end of a swing; Ilda's fireballs land when they arrive.
- Each companion levels up separately and earns a talent point every 2 levels. Each one has two specs:

  | Companion | Specs |
  |---|---|
  | Bram (Guardian) | Bulwark or Vengeance |
  | Rook (Warrior) | Berserker or Executioner |
  | Vess (Rogue) | Assassin or Poisoner |
  | Ilda (Pyromancer) | Inferno or Ember Storm |

  Examples include Shield Bash, Execute, Cleave, poison stacks, Pyroblast and splash damage.
- **Gold upgrades:** every companion has a Weapon (+12% damage per rank) and Armor (+10% health per rank) with no rank limit. Each rank costs 60% more than the last, so gold always has a use.

## Other progression

- **Gear.** Enemies drop items for six slots in five rarities. Enchant equipped items with gold for +10% stats per level.
- **Item mastery.** Every item teaches a skill. Clear stages with it equipped to master it, and the skill is yours for good.
- **The sanctum.** Healing earns gold. Buildings earn gold every second, and blessings are one-time upgrades. Buildings keep earning for up to 8 hours while you're away.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, +5 Cleric talent points, win the current stage, unlock the next dungeon, drop an item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
