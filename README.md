# Mendwright

A small healing game in a single HTML file. It mixes the party healing of **Master Healer Kale** and **Mini Healer** with WoW-style talent trees, a town you build up, idle expeditions while you're away, and an **Astlibra**-style item mastery system.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press its key. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Action bar.** Twelve slots bound to `1`–`6`, `E`, `F`, `R`, `T`, `Q` and `Y`. New spells go to the first free slot (the Mana Potion prefers `Q`). Click **Edit keybinds** to rearrange: drag a spell from your spellbook onto a key, drag between keys to swap, or drag a key back to the spellbook to clear it. Clicking a spell and then a key works too.
- **Gold.** Every enemy drops gold when it dies. Coins pop out and fly to your Cleric, and a boss bursts into a shower of them. Tougher monsters and deeper dungeons pay more.
- **Targeting.** A gold ring marks who your next spell will hit. While you cast, a green glow builds on the ally about to receive the heal.
- **Mana.** Spell costs grow with your Cleric's level and average item level. Spell power makes each point of mana heal more, and regeneration buys more casts. Mana is loose on dungeons you've outgeared, and you'll feel it when pushing into a new one.
- **Dungeons.** Eight dungeons, each 5–10 stages of monster packs ending in a boss. Health and mana carry over between stages, with a short rest. Every dungeon has a rule of its own (poison, a silenced spell, scorching air, weaker healing, low mana, an early berserk timer). Each new dungeon is much harder than the last, so you farm until you're ready, then choose to push on.
- **You lose** if you die or the rest of the party dies. Rewards from stages you cleared are kept. With *Repeat dungeon* on, the run starts again by itself.

## Why heal actively

- **Devotion.** Each heal that lands builds Devotion. Overhealing, or leaving hurt allies unhealed, drains it. Devotion scales the gold from every kill and the experience and loot from every stage, from ×0.5 when you idle up to ×3. It fades slowly on its own and gains less the higher it gets, so steady, efficient healing holds it around ×1.5–2. Reaching ×3 takes a lot of work.
- **Pleas.** Every minute or so, a companion glows gold and pleads for help. Heal them within 6 seconds for a random reward: a gold windfall, a ×5 Gold Frenzy, ×2 party damage, a burst of experience, a rare-or-better relic, or (rarely) a talent point.

## Cleric talents

- You start with only **Heal**. The other eight spells are learned in the talent trees.
- Three WoW-style trees: **Holy** (Heal, Flash Heal, Prayer), **Discipline** (Ward, Purify, Sanctuary, the tank) and **Devotion** (mana, Renew, Meditate, Blessing).
- Most talents take 5–10 ranks of small bonuses. Ranks 1–5 cost 1 point and later ranks cost 2. Major talents (2–3 points) and new spells (3–4 points) sit between them.
- Deeper rows need points spent in that tree first: 2 per row.
- Talent points are rare: 1 every 2 Cleric levels, plus 1 for each first dungeon clear. Resetting is free.

## The party

- Companions attack on their own timers. Every hit has its own damage, attack speed, critical chance and critical damage. Melee hits land at the end of a swing; Vess's arrows and Ilda's fireballs land when they arrive.
- Each companion levels up separately and earns a talent point every 2 levels. Each one has two specs:

  | Companion | Specs |
  |---|---|
  | Bram (Guardian) | Bulwark or Vengeance |
  | Rook (Warrior) | Berserker or Executioner |
  | Vess (Hunter) | Marksman or Venom |
  | Ilda (Mage) | Fire or Frost |

  Examples include Shield Bash, Execute, Cleave, poison stacks, Pyroblast and splash damage.
- **Companion attacks.** The third column of every spec is a new attack the companion fires on its own cooldown, on top of their normal hits. Learn it (2 points), then improve it with the talents right below: more damage, a shorter cooldown, and a major upgrade at the bottom.

  | Companion | Attacks | Major upgrade |
  |---|---|---|
  | Bram | Shield Slam (200%, Bram takes 20% less damage for 4s) · Thunder Clap (130% to every enemy) | Concussion stuns and interrupts · Aftershock slows enemy attacks |
  | Rook | Whirlwind (3 spins of 70% to every enemy) · Mortal Strike (300%) | Bladestorm: 5 spins · Decapitate: triple damage below 35% health |
  | Vess | Aimed Shot (300%, always critical) · Venom Volley (80% to every enemy plus 2 poison stacks) | Piercing Shot hits every enemy · Rain of Arrows fires a second wave |
  | Ilda | Flamestrike (150% to every enemy, then a burn) · Frostbolt (200%, slows attacks by 30%) | Wildfire doubles the burn · Deep Freeze freezes and interrupts |
- **Damage meter.** Under the action bar, the damage meter ranks the party by damage per second over the current run, with each member's share. Use it to spot who is falling behind and push their gear, training or talents.
- **Gear.** Each companion has three gear slots (weapon, armor, charm), with damage, health, attack speed and critical stats. When you select party gear in the Armory, it shows the change in damage per second or health for each companion.
- **Training.** Every companion has Weapon Training (+2% damage per rank) and Endurance Training (+2% health per rank). There's no rank limit, and ranks add up, so 10 ranks is +20%. Each rank costs 50% more than the last, which keeps training roughly level with the companion's talents.

## Other progression

- **Gear.** Enemies drop items for the Cleric's six slots and the companions' three, in five rarities. The header shows your **party item level**, the average across all 18 slots. **Equip best items** fills every slot automatically: armor goes to the tank first, and weapons and charms go to the hardest hitters first. Enchant equipped items with gold for +10% stats per level.
- **Item mastery.** Every item teaches a skill. Clear stages with it equipped to master it, and the skill is yours for good.
- **The Town.** Every stage drops materials from its dungeon (Rat Tails, Bog Moss and so on), with more at high Devotion. The Town tab shows your town as a pixel-art map with seven empty plots. Click a plot to see what it would do, and build it: the building rises out of the ground and stays on the map, gaining a banner at level 4 and gold trim at level 8. Buildings go up to level 8 and cost gold plus materials. Level 1 uses materials from the first dungeon, level 2 from the second, and so on, so pushing deeper unlocks the next tier:

  | Building | What it does |
  |---|---|
  | Acolyte Cloister | Hires and upgrades the Acolyte |
  | Infirmary | Better resting between stages; fallen allies return with more health |
  | Herb Garden | Mana potions you drink mid-fight with Q |
  | Chapel | Starts each run with Devotion; Devotion fades slower |
  | Library | More experience |
  | Smithy | Cheaper, stronger enchanting |
  | Barracks | Cheaper training |

  The Town tab also sells one-time blessings for gold.
- **Expeditions.** Once you build the Acolyte Cloister, an Acolyte heals the party in the background (weakly at first). While the game is closed or in another tab, the Acolyte leads the party through the dungeon you're in, if you've cleared it, otherwise your deepest clear. They run at 20–55% of your active pace for up to 8 hours and bring back gold, experience, materials and items.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, +5 Cleric talent points, +20 materials, simulate 1 hour away, win the current stage, unlock the next dungeon, drop an item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
