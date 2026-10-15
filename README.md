# Mendwright

A small healing game in a single HTML file. It mixes the party healing of **Master Healer Kale**, WoW-style talent trees, and **Mini Healer** with Cookie Clicker–style idle income and an **Astlibra**-style item mastery system.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press its number. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Targeting.** A gold ring marks who your next spell will hit. While you cast, a green glow builds on the ally about to receive the heal.
- **Mana.** Spell costs grow with your healing power. Mana is loose on dungeons you've outgeared, and you'll feel it when pushing into a new one.
- **Dungeons.** Eight dungeons, each 5–10 stages of monster packs ending in a boss. Health and mana carry over between stages, with a short rest. Every dungeon has a rule of its own (poison, a silenced spell, scorching air, weaker healing, low mana, an early berserk timer). Each new dungeon is much harder than the last, so you farm until you're ready, then choose to push on.
- **You lose** if you die or the rest of the party dies. Rewards from stages you cleared are kept. With *Repeat dungeon* on, the run starts again by itself.

## Why heal actively

- **Devotion.** Each heal that lands builds Devotion. Overhealing, or leaving hurt allies unhealed, drains it. Devotion scales the gold, experience and loot from every stage, from ×0.5 when you idle up to ×3. It fades slowly on its own and gains less the higher it gets, so steady, efficient healing holds it around ×1.5–2. Reaching ×3 takes a lot of work.
- **Heals pay income.** Every heal that actually restores health pays a few seconds of your buildings' gold per second, so healing keeps pace as your income grows. Tithe upgrades raise it from 1 second to 20.
- **Pleas.** Every minute or so, a companion glows gold and pleads for help. Heal them within 6 seconds for a random reward: a gold windfall, a ×5 Gold Frenzy, ×2 party damage, a burst of experience, a rare-or-better relic, or (rarely) a talent point.

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
- **Gear.** Each companion has three gear slots (weapon, armor, charm), with damage, health, attack speed and critical stats. When you select party gear in the Armory, it shows the change in damage per second or health for each companion.
- **Training.** Every companion has Weapon Training (+2% damage per rank) and Endurance Training (+2% health per rank). There's no rank limit, and ranks add up, so 10 ranks is +20%. Each rank costs 50% more than the last, which keeps training roughly level with the companion's talents.

## Other progression

- **Gear.** Enemies drop items for the Cleric's six slots and the companions' three, in five rarities. The header shows your **party item level**, the average across all 18 slots. **Equip best items** fills every slot automatically: armor goes to the tank first, and weapons and charms go to the hardest hitters first. Enchant equipped items with gold for +10% stats per level.
- **Item mastery.** Every item teaches a skill. Clear stages with it equipped to master it, and the skill is yours for good.
- **The sanctum.** Healing earns gold. Buildings earn gold every second, and blessings are one-time upgrades. Buildings keep earning for up to 8 hours while you're away.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, +5 Cleric talent points, win the current stage, unlock the next dungeon, drop an item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
