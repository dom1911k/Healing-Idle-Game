# Mendwright

A small healing game in a single HTML file. It mixes the party healing of **Master Healer Kale** and **Mini Healer** with WoW-style talent trees, a town you build up, idle expeditions while you're away, and an **Astlibra**-style item mastery system.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press its key. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Action bar.** Twelve slots bound to `1`–`6`, `E`, `F`, `R`, `T`, `Q` and `Y`. New spells go to the first free slot (the Mana Potion prefers `Q`). Click **Edit keybinds** to rearrange: drag a spell from your spellbook onto a key, drag between keys to swap, or drag a key back to the spellbook to clear it. Clicking a spell and then a key works too.
- **Gold.** Every enemy drops gold when it dies. Coins pop out and fly to your Cleric, and a boss bursts into a shower of them. Tougher monsters and deeper dungeons pay more.
- **Targeting.** A gold ring marks who your next spell will hit. While you cast, a green glow builds on the ally about to receive the heal.
- **Mana.** Spell costs grow with your Cleric's level and average item level. Spell power makes each point of mana heal more, and regeneration buys more casts. Mana is loose on dungeons you've outgeared, and you'll feel it when pushing into a new one. Trying to cast without enough mana shows a quiet blue *Not enough mana* on the mana bar, and when you're running low, Meditate and the Mana Potion glow blue on the action bar.
- **Dungeons.** The Dungeons tab is a map of the descent: each dungeon has a painted banner with its boss, its rule, your progress through its stages, and how hard it is for your party's level. Eight dungeons, each 5–10 stages of monster packs ending in a boss. Health and mana carry over between stages, with a short rest. Every dungeon has a rule of its own (poison, a silenced spell, scorching air, weaker healing, low mana, an early berserk timer). Each new dungeon is much harder than the last, so you farm until you're ready, then choose to push on.
- **Debuffs.** Poison ramps up with every tick, a hex halves the healing its target receives, and wolves cause short bleeds. Purify removes all of them. A Ward that is still holding makes its target resist new poisons and hexes.
- **Boss telegraphs.** When a boss starts a big ability, the cast bar names the target, a red marker hovers over that hero and their party frame pulses red. Wave attacks mark the whole party. Later bosses add **Doom**, a slow cast that hits one ally for a huge amount: shield them with Ward or top them up in time.
- **Boss second phases.** At half health every boss changes: Gnasher calls in rats, the Mire Hag poisons everyone, the Grave Warden raises skeletons, Ashjaw sets the floor on fire, Thornmother weakens healing and summons wisps, the Iron Penitent casts Doom at once and speeds up, and so on. Each dungeon card says what to expect.
- **Elites.** Now and then a stage holds an elite with a gold crown and one trait: Shielded (a barrier soaks damage first), Enraged (faster below half health), Mender (heals its allies) or Venomous (poisons). Elites have four times the health and always drop an uncommon-or-better item, extra materials and five times the gold.
- **Peril.** Once you've cleared a dungeon and unlocked the next one, you can raise its Peril on the Dungeons tab. Each level gives enemies ×1.6 health and ×1.5 damage, and gives ×1.3 rewards, +50% of that dungeon's materials, items two item levels higher and more elites. The cap keeps a Perilous old dungeon's rewards below those of your deepest dungeon, so it's a way to farm materials, not to skip ahead.
- **Wipe report.** When the party falls, the summary explains what happened: who died to what and what would have helped, whether the enemies went berserk, how much of the fight you were out of mana, how much healing was overheal, and anything left unspent.
- **You lose** if you die or the rest of the party dies. Rewards from stages you cleared are kept. With *Repeat dungeon* on, the run starts again by itself.

## Look and feel

- **Every dungeon has its own scenery:** sewer pipes and a murky channel, a bog with hanging roots and drifting fog, a crypt of burial niches and candles, glowing cracks over a lava channel, a moonlit forest, barred cells with swaying chains, a flooded nave under stained glass, and a starry void with a black sun.
- Characters and monsters get light-and-shadow shading. Hits knock targets back, Vess and Ilda recoil when they fire, fallen heroes topple before their grave rises, and every boss arrives with a name card. Bosses have been redrawn, including the Grave Warden, Thornmother, Ashjaw, the Iron Penitent, the Leviathan and the Eclipse Seraph.
- The town sits under a dusk sky with drifting clouds, birds, a windmill and a castle on the ridge. It has cobbled streets, a plaza fountain, lamp posts, a pond and villagers who walk the main street (more of them as the town grows). Buildings are shaded and outlined, chimneys smoke, and buildings gain flower boxes at level 3 and an annex at level 5.

## Getting started

- One-time hints appear the first time each system matters: targeting, Devotion, pleas, debuffs, boss telegraphs, mana, talent points, promotions, the Town, elites, boss phases, Peril and sets.
- A **Next** line under the arena header suggests the most useful thing to do now, like choosing a spell, equipping upgrades, spending points, promoting someone or building in the Town. Click it to jump to the right tab.
- **Sound.** Short synthesized effects for heals, crits, coins, hits, boss warnings, level-ups and achievements. Use the speaker button and slider in the header to mute or set the volume.

## Why heal actively

- **Devotion.** Each heal that lands builds Devotion. Overhealing, or leaving hurt allies unhealed, drains it. Devotion scales the gold from every kill and the experience and loot from every stage, from ×0.5 when you idle up to ×3. It fades slowly on its own and gains less the higher it gets, so steady, efficient healing holds it around ×1.5–2. Reaching ×3 takes a lot of work.
- **Ward, Purify and Renew pull their weight.** Damage a Ward soaks counts as effective healing for Devotion. Purify refunds half its mana whenever it removes something and always counts as a useful cast. Renew is cheaper and stronger, and its overhealing jumps to the most injured ally at half strength.
- **Pleas.** Every minute or so, a companion glows gold and pleads for help. Heal them within 6 seconds for a random reward: a gold windfall, a ×5 Gold Frenzy, ×2 party damage, a burst of experience, a rare-or-better relic, or (rarely) a talent point.

## Spells

- You start with only **Heal**. The other eight spells don't cost talent points: the **first clear of each dungeon** lets you choose one of three new spells. The ones you pass on stay on offer for your next first clear. Spells come up in the order their talents open in the trees: Flash Heal, Purify and Renew first, then Ward and Meditate, then Prayer, then Sanctuary and Blessing.
- With *Repeat dungeon* on, the next run waits until you've chosen. You can also choose from the Talents tab, which always shows which spells your next first clear will offer.

## Cleric talents

- The Talents tab shows the three trees as crests, each with the spells it improves and the points you've spent in it.
- Spells aren't in the trees. Talents with a small spell icon improve that spell and open once you know it; until then they show which spell they need. Every row also has talents that work without any new spell, and each tree ends in a capstone (Miracle, Inner Fortress, Zealot).
- New talents: **Lifeline** (stronger heals on allies below 40% health), **Miracle** (critical heals refund mana), **Steadfast Faith** (Devotion fades slower), **Last Rites** (once per stage, an ally survives a killing blow) and **War Chant** (companions attack faster).
- Three WoW-style trees: **Holy** (Heal, Flash Heal, Prayer), **Discipline** (Ward, Purify, Sanctuary, the tank) and **Devotion** (mana, Renew, Meditate, Blessing).
- Most talents take 5–10 ranks of small bonuses. Ranks 1–5 cost 1 point and later ranks cost 2. Major talents (2–3 points) sit between them.
- Deeper rows need points spent in that tree first: 2 per row.
- Talent points are rare: 1 every 2 Cleric levels, plus 1 for each first dungeon clear. Resetting is free.

## The party

- Companions attack on their own timers. Every hit has its own damage, attack speed, critical chance and critical damage. Melee hits land at the end of a swing; Vess's arrows and Ilda's fireballs land when they arrive.
- The Party tab shows each member as a portrait card in their class color, with a badge when they have talent points to spend. The party frames in the arena show the same portraits and colors.
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
- **Damage meter.** Under the action bar, the damage meter ranks the party by damage per second over the current run, with each member's share. Use it to spot who is falling behind and push their gear, promotions or talents.
- **Gear.** Each companion has three gear slots (weapon, armor, charm), and every companion item belongs to one companion: Bram wears plate and swings swords, maces and warhammers; Rook uses greataxes, claymores and halberds; Vess uses bows and crossbows, leathers and quivers; Ilda uses spellstaffs, wands and grimoires, robes and orbs. Each base has its own icon and items are named from their material (iron, yew, silk, drakehide and so on) and their main stat. Selecting one in the Armory shows what it changes for its owner.
- **Synergies.** Companions leave marks on enemies that the rest of the party exploits, shown as colored pips over each enemy: sunder (red), mark (gold), poison (green), burn (orange), chill (blue) and stun (white). Each spec has a synergy talent in its fourth row: Bram's *Sunder Armor* and *Concussive Force*, Rook's *Shatter* and *Opportunist*, Vess's *Mark for Death* and *Festering Wounds*, Ilda's *Volatile Venom* and *Brittle Ice*. Companion gear can also roll *Damage vs. Slowed or Stunned* and *Damage vs. Poisoned or Burning*.
- **Promotions.** Each party member climbs seven ranks (Recruit, Veteran, Elite, Champion, Hero, Legend, Paragon). Each rank unlocks at a level (5, 10, 15 and so on) and costs six times the last. Every rank gives a stat boost (+12% damage and health for companions, +8% healing and max mana for the Cleric), a **signature perk** and **upgraded gear** you see in combat, on the party frames and on the portraits.

  | Member | Veteran | Elite | Champion | Hero | Legend | Paragon |
  |---|---|---|---|---|---|---|
  | Bram | Shield Wall | Intercept boss attacks | Bulwark (party −5% damage) | Unyielding | Retribution | Aegis Aura (party −8% damage) |
  | Rook | Second Swing | Battle Cry | Bloodthirst | Whirling Steel | Rampage | Executioner |
  | Vess | Hawk Eye | Twin Arrows | **Hunting Hawk** pet | Keen Shots | Piercing Arrows | Deadeye |
  | Ilda | Kindled | Mana Font | **Fire Familiar** pet | Arcane Surge | Inferno | Meteor Storm |
  | Cleric | Devout | Halo | Guardian Angel | Radiance | Divine Favor | Ascension |

  Gear changes with every rank: Bram's armor goes from steel to polished silver to gold, Rook's tunic becomes chainmail and then red-gold plate, Vess's bow turns gold and then silver, Ilda's robes deepen to arcane blue and the staff's flame turns blue, and the Cleric's robes brighten. Capes come at Elite, auras at Hero, halos at Legend and wings of light at Paragon. Colored rank pips sit over each hero in combat. The Party tab shows a portrait for every rank, a before-and-after preview of the next promotion and the full perk list.

## Other progression

- **Gear.** Enemies drop items for the Cleric's six slots and the companions' three, in five rarities. The header shows your **party item level**, the average across all 18 slots. **Equip best items** fills every slot automatically: armor goes to the tank first, and weapons and charms go to the hardest hitters first. Enchant equipped items with gold for +10% stats per level.
- **Item sets.** Each companion and the Cleric has a three-piece set that sometimes drops in place of a rare-or-better item (set pieces are always epic, with teal names). Two pieces give a stat bonus, and three unlock a synergy: Bram's hits sunder armor, Rook always crits slowed or stunned enemies, Vess's crits mark enemies for 8 seconds, Ilda's fireballs chill, and the Cleric's heals on low allies also shield them. The item view shows the set's pieces and bonuses.
- **Looks.** Promotions show on the battlefield: a cape in the companion's color from Elite, gold trim at Champion, a glowing aura and rising motes at Hero, and a halo at Legend. Epic or legendary armor gives a colored outline, and epic or legendary weapons sparkle.
- **Loot filter.** In the Armory, choose to auto-sell drops below a rarity (upgrades are never sold), and optionally equip upgrades as they drop. When the bag is full, the weakest non-upgrade is sold to make room.
- **Merchant.** Once you build a Market, the Armory sells sealed items for the deepest dungeon you've reached: a Supply Crate (any rarity), a Gilded Coffer (rare or better) and a Royal Reliquary (epic or better, 20% legendary).
- **Elixirs.** As the Herb Garden grows, the Dungeons tab sells three elixirs (+25% party damage, 15% less damage taken, +40% mana regeneration). Each lasts 10 minutes of fighting and stacks up to an hour. Their price scales with your deepest dungeon.
- **Achievements.** Fifteen achievements, such as clearing a dungeon without a death, slaying ten elites, wearing a full set or clearing at Peril 3. Each grants a small permanent bonus: healing, damage, gold, experience, mana or a talent point. They're listed in the Chronicle with progress bars.
- **Chronicle.** Healing by spell for this run or all time, with share, overheal and casts, plus damage taken, party deaths, debuffs cleansed and deaths per dungeon.
- **Item mastery.** Every item teaches a skill. Clear stages with it equipped to master it, and the skill is yours for good.
- **The Town.** Every stage drops materials from its dungeon (Rat Tails, Bog Moss and so on), with more at high Devotion. The Town tab shows your town as a pixel-art map with eight empty plots. Click a plot to see what it would do, and build it: the building rises out of the ground and stays on the map, gaining a banner at level 4 and gold trim at level 8. Buildings go up to level 8 and cost gold plus materials. Level 1 uses materials from the first dungeon, level 2 from the second, and so on, so pushing deeper unlocks the next tier:

  | Building | Every level | Unlocks |
  |---|---|---|
  | Acolyte Cloister | A stronger Acolyte and faster expeditions | Lv 3 the Acolyte cleanses debuffs · Lv 5 the Acolyte shields Bram |
  | Infirmary | Better resting; fallen allies return with more health | Lv 3 Triage: allies below 25% take less damage · Lv 6 Second Wind: once per stage the first ally to fall gets back up |
  | Herb Garden | One more mana potion per run | Lv 2/4/6 the three elixirs · Lv 3 Healing Draught (heals the party for 25%, on F) · Lv 7 a second draught |
  | Chapel | Start with Devotion; Devotion fades slower | Lv 3 Chapel Bell (+35 Devotion once per run, on R) · Lv 6 Devotion never falls below 20% |
  | Library | More experience | Lv 3 and 7 a bonus Cleric talent point · Lv 5 first clears offer four spells |
  | Smithy | Cheaper, stronger enchanting | Lv 3 Reforge (reroll an item's stats) · Lv 5 every drop is one item level higher |
  | Barracks | Cheaper promotions | Lv 2 Battle Stances (Aggressive, Balanced or Defensive, in the Party tab) · Lv 4 +20% experience |
  | Market | Cheaper sealed items | Lv 1/3/5 Supply Crates, Gilded Coffers and Royal Reliquaries |

  Clicking a building shows its milestones, with what's unlocked and what comes next.

  The Town tab also sells one-time blessings for gold.
- **Expeditions.** Once you build the Acolyte Cloister, an Acolyte heals the party in the background (weakly at first). While the game is closed or in another tab, the Acolyte leads the party through the dungeon you're in, if you've cleared it, otherwise your deepest clear. They run at 20–55% of your active pace for up to 8 hours and bring back gold, experience, materials and items.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, +5 Cleric talent points, +20 materials, simulate 1 hour away, win the current stage, unlock the next dungeon, drop an item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
