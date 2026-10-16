# Mendwright

A small healing game in a single HTML file. It mixes the party healing of **Master Healer Kale** and **Mini Healer** with WoW-style talent trees, a town you build up, idle expeditions while you're away, and an **Astlibra**-style item mastery system.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a hero in the battle scene or a party frame to target them, then click a spell or press its key. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Action bar.** Twelve slots bound to `1`–`6`, `E`, `F`, `R`, `T`, `Q` and `Y`. New spells go to the first free slot (the Mana Potion prefers `Q`). Click **Edit keybinds** to rearrange: drag a spell from your spellbook onto a key, drag between keys to swap, or drag a key back to the spellbook to clear it. Clicking a spell and then a key works too.
- **Gold.** Every enemy drops gold when it dies. Coins pop out and fly to your Cleric, and a boss bursts into a shower of them. Tougher monsters and deeper dungeons pay more.
- **Targeting.** A gold ring marks who your next spell will hit. While you cast, a green glow builds on the ally about to receive the heal.
- **Mana.** Spell costs grow with your Cleric's level and average item level. Spell power makes each point of mana heal more, and regeneration buys more casts. Mana is loose on dungeons you've outgeared, and you'll feel it when pushing into a new one. Trying to cast without enough mana shows a quiet blue *Not enough mana* on the mana bar, and when you're running low, Meditate and the Mana Potion glow blue on the action bar.
- **Dungeons.** The Dungeons tab is a map of the descent: each dungeon has a painted banner with its boss, its rule, your progress through its stages, and how hard it is for your party's level. Twelve dungeons in two acts, each 5–10 stages of monster packs ending in a boss. Health and mana carry over between stages, with a short rest. Every dungeon has a rule of its own (poison, a silenced spell, scorching air, weaker healing, low mana, an early berserk timer). Each new dungeon is much harder than the last, so you farm until you're ready, then choose to push on.
- **Readable battlefield text.** Banners, ability names, level-ups, boss name cards and town labels use a crisp pixel font with an outline.
- **Debuffs.** Poison ramps up with every tick, a hex cuts the healing its target receives by 30% for 6 seconds, and wolves cause short bleeds. There are no cleansing spells: debuffs run their course. A Ward that is still holding makes its target resist new poisons and hexes, and shields soak the damage debuffs deal.
- **Act II: The Hollow Crown.** Beating the Eclipse Seraph opens four deeper dungeons with new monsters (cave spiders that poison, wraiths that wither, crystal golems that pound the tank, gargoyles), new scenery, new music and new materials:

  | Dungeon | Rule | Boss | Boss checks |
  |---|---|---|---|
  | IX Webbed Depths | **Venom**: poisons ramp twice as fast | Broodmother Xyth | Soul Chain, Plague; spiders hatch at half health |
  | X Crystal Caverns | **Shard Rain**: shards hit the party every 12 seconds | Crystal Colossus | Prismatic Mark, Skull Crusher |
  | XI Frostveil Hollow | **Bitter Cold**: casts and channels take 20% longer | The Rime Queen | Frost Theft, Necrotic Grip, Doom |
  | XII The Hollow Crown | **The Void**: 25% less max mana | The Hollow King | everything, plus Soul Chain and Frost Theft |

  - **Soul Chain** links two allies for 10 seconds (a chain is drawn between them): half the damage one takes also hits the other.
  - **Prismatic Mark**: for 6 seconds, healing that ally heals the boss for twice as much. Shield them or let them wait.
  - **Frost Theft** steals every heal over time and shield on the party and turns them into a shield for the boss. Hold your heals over time until it lands.
- **Ascension.** Once you beat the Hollow King, the Dungeons tab lets you **ascend**: start over from the sewers for permanent **Echoes**. You keep achievements, stats, Echoes and the Echo Altar; gold, levels, dungeons, Town, gear, promotions, talents and spells reset. Each cycle's enemies are 25% tougher and pay 30% more. Spend Echoes at the **Echo Altar** on Might (party damage), Life (party health), Grace (healing), Fortune (gold and experience), Home (start each cycle with buildings already built) and Memory (keep your first spells).
  - **Ascension challenges.** Before you ascend, you can curse the next cycle: Broken Wards (your shield spell is sealed), Wrath (bosses start in phase 2), Frail Guardian (Bram has 40% less health), Dim Light (20% weaker healing), Swarm (one more enemy per pack) and Fury (enemies attack 20% faster). Each curse adds 15–25% to the Echoes that cycle pays when you ascend again.
  - **Cosmetics.** Spend Echoes once on a Golden or Void aura under the party, Azure or Ember spell effects, a war banner for Bram, a floating crown for your healer, or glowing footsteps. Switch them on and off any time.
- **Bosses test the healer.** Bosses act more often the deeper you go, and from the second dungeon on they bring checks you have to answer:
  - **Plague** (green countdown badge): heal the target to full health within 7 seconds to cure it, or it bursts on the whole party. A Ward or Bone Shield on the target blocks it before it lands.
  - **Necrotic Grip**: soaks up the next heals on that ally (the badge shows how much is left), so you have to heal through it.
  - **Skull Crusher**: a slow, telegraphed blow on Bram for five times a normal hit. Shield him, Barkskin him or top him up before it lands.
- **Boss telegraphs.** When a boss starts a big ability, the cast bar names the target, a red marker hovers over that hero and their party frame pulses red. Wave attacks mark the whole party. Later bosses add **Doom**, a slow cast that hits one ally for a huge amount: shield them with Ward or top them up in time.
- **Boss second phases.** At half health every boss changes: Gnasher calls in rats, the Mire Hag poisons everyone, the Grave Warden raises skeletons, Ashjaw sets the floor on fire, Thornmother weakens healing and summons wisps, the Iron Penitent casts Doom at once and speeds up, and so on. Each dungeon card says what to expect.
- **Elites.** Now and then a stage holds an elite with a gold crown and one trait: Shielded (a barrier soaks damage first), Enraged (faster below half health), Mender (heals its allies) or Venomous (poisons). Elites have four times the health and always drop an uncommon-or-better item, extra materials and five times the gold.
- **Peril.** Once you've cleared a dungeon and unlocked the next one, you can raise its Peril on the Dungeons tab. Each level gives enemies ×1.6 health and ×1.5 damage, and gives ×1.3 rewards, +50% of that dungeon's materials, items two item levels higher and more elites. The cap keeps a Perilous old dungeon's rewards below those of your deepest dungeon, so it's a way to farm materials, not to skip ahead.
- **Wipe report.** When the party falls, the summary explains what happened: who died to what and what would have helped, whether the enemies went berserk, how much of the fight you were out of mana, how much healing was overheal, and anything left unspent.
- **You lose** if you die or the rest of the party dies. Rewards from stages you cleared are kept. With *Repeat dungeon* on, the run starts again by itself.

## Look and feel

- **Every dungeon has its own scenery:** sewer pipes and a murky channel, a bog with hanging roots and drifting fog, a crypt of burial niches and candles, glowing cracks over a lava channel, a moonlit forest, barred cells with swaying chains, a flooded nave under stained glass, and a starry void with a black sun.
- **Incoming heals, WoW style.** While you cast (or channel Drain Life), the target's health bar shows a bright pulsing segment for the health your spell will restore when it lands, on the party frame and on the small bar over the hero. Group heals like Prayer and Soul Harvest show it on everyone. Necrotic Grip and healing cuts are taken into account.
- **Casting.** A rune circle in your class color turns under your healer and brightens as the cast fills, light rises around them, sparks gather and the orb on the staff grows, and the circle flares when the spell goes off.
- **Lighting.** Each dungeon sits under its own darkness, with light pooling around torches, heroes, enemies and spells, and a soft color grade (green in the sewers, cold blue in the crypt, ember orange in the Cinder Pit, magenta under the Hollow Crown). A foreground layer of roots, chains, webs or icicles slides past faster than the background while the party walks. Spell sparks glow, heal beams have soft edges and a ring of light at the target's feet, and health bars show a pale chunk for the health just lost before it drains away.
- Characters and monsters get light-and-shadow shading. Hits knock targets back, Vess and Ilda recoil when they fire, fallen heroes topple before their grave rises, and every boss arrives with a name card. Bosses have been redrawn, including the Grave Warden, Thornmother, Ashjaw, the Iron Penitent, the Leviathan and the Eclipse Seraph.
- The town sits under a dusk sky with drifting clouds, birds, a windmill and a castle on the ridge. It has cobbled streets, a plaza fountain, lamp posts, a pond and villagers who walk the main street (more of them as the town grows). Buildings are shaded and outlined, chimneys smoke, and buildings gain flower boxes at level 3 and an annex at level 5.

## Getting started

- One-time hints appear the first time each system matters: targeting, Devotion, pleas, debuffs, boss telegraphs, mana, talent points, promotions, the Town, elites, boss phases, Peril, sets, Plague, Necrotic Grip, Skull Crusher and losing the tank.
- A **Next** line under the arena header suggests the most useful thing to do now, like choosing a spell, equipping upgrades, spending points, promoting someone or building in the Town. Click it to jump to the right tab.
- **Sound and music.** Casting sounds follow your class: a Priest's choir swells on a major chord with rising chimes, a Druid's cast is wind through leaves with a breathy wooden flute and wind chimes, and an Occultist's is a low droning chant with a dissonant whisper and a slow heartbeat. Heals sound like your class too: a Priest's bell, a Druid's wooden pluck, an Occultist's dark swell, each with a bright snap on top. Critical heals add a rising chime. Casts hum upward as they charge, heals over time tick softly, shields ring like glass and hits land with a thump. There are also effects for coins, boss warnings, level-ups and achievements, and a chiptune song for every dungeon. Each song has four parts (the main tune, the tune with a harmony line, a bridge with new chords and arpeggios, then the tune an octave higher with echoes and drum fills), so it runs about four times longer before repeating (bouncy in the Sewers, eerie in the Crypt, driving in the Cinder Pit, a march in the Iron Bastille and so on). Boss fights play the theme faster with heavier drums. The ♪ button toggles music, the speaker button mutes everything and the slider sets the volume.
- **Phones.** On narrow screens the party frames sit three to a row, the tabs wrap into two rows and empty action-bar slots hide until you edit keybinds. **Hold a party frame** (or right-click it on a computer) for a quick-cast ring of your spells around it: slide onto a spell and let go, or let go and tap one.

## Why heal actively

- **Devotion.** Each heal that lands builds Devotion. Overhealing, or leaving hurt allies unhealed, drains it. Devotion scales the gold from every kill and the experience and loot from every stage, from ×0.5 when you idle up to ×3. It fades slowly on its own and gains less the higher it gets, so steady, efficient healing holds it around ×1.5–2. Reaching ×3 takes a lot of work.
- **Ward and Renew pull their weight.** Damage a Ward soaks counts as effective healing for Devotion. Renew is cheaper and stronger, and its overhealing jumps to the most injured ally at half strength.
- **Pleas.** Every minute or so, a companion glows gold and pleads for help. Heal them within 6 seconds for a random reward: a gold windfall, a ×5 Gold Frenzy, ×2 party damage, a burst of experience, a rare-or-better relic, or (rarely) a talent point.

## Spells

- You start with only **Heal**. The other eight spells don't cost talent points: the **first clear of each dungeon** lets you choose one of three new spells. The ones you pass on stay on offer for your next first clear. Spells come up in the order their talents open in your class's trees (for the Priest: Flash Heal, Circle of Healing and Renew first, then Ward and Meditate, then Prayer, then Sanctuary and Blessing).
- With *Repeat dungeon* on, the next run waits until you've chosen. You can also choose from the Talents tab, which always shows which spells your next first clear will offer.

## Healer classes and talents

- **No more cleansing.** The old cleanse spells (Purify, Remove Corruption, Purge) are gone. That spell slot is now a heal for each class: the Priest's **Circle of Healing** (instant, heals the three most injured allies, 8-second cooldown), the Druid's **Nourish** (a 1.6-second efficient heal, 30% stronger for each of your heals over time on the target) and the Occultist's **Death Coil**. Their talents were reworked to match (Circle of Light, Improved Nourish, Improved Death Coil). The Clean Hands achievement became Iron Will (absorb 25,000 damage with shields), and the cleanse bounty became saving allies below 10% health.

- Pick a healer class in the Talents tab, in the spirit of Mini Healer's Priest, Druid and Occultist trees. Switching is free. **Each class keeps its own talents and its own spell choices**: a class you haven't played yet starts with one spell pick per dungeon you've already cleared, so you choose its spells from that class's offer. Switching back restores that class's setup. Each class renames and reworks your spells, has its own passive, its own look, its own reward resource (Devotion, Harmony or Dread) and three talent trees of its own:

  | Class | Resource | How it plays |
  |---|---|---|
  | **Priest** | **Holy Power** (up to 3) | Heal and Flash Heal build Holy Power. Prayer spends it for +25% healing per point and is instant at 3. A Ward cast at 3 also shields the rest of the party for half. Radiant Overflow turns 30% of overhealing into shields. |
  | **Druid** | Heals over time | Plant Rejuvenation (stacks twice) and Regrowth, then **Swiftmend eats the strongest one** to heal for everything it had left plus 30%. **Tree of Life** (replaces Mark of the Wild): 15 seconds where heals over time heal 40% more, Regrowth is instant and the party deals 15% more damage, and you turn into a tree. Barkskin, instant Wild Growth, Tranquility. Heal-over-time ticks restore mana. |
  | **Occultist** | **Souls** (up to 5) | You heal by hurting. **Drain Life is a 3-second channel** that drains the front enemy and pours it into the ally you chose; it does nothing with no enemy in reach. **Leech Seed goes on an enemy** and heals your chosen ally every second as it damages. **Blood Bolt** costs your own health instead of mana. **Death Coil** (instant, 6-second cooldown) strikes the front enemy and heals the ally you chose for even more. Every kill and every finished Drain Life gives a Soul, and **Soul Harvest** spends them all (weak with none, huge with five). **Unholy Ground** damages every enemy each second, and Siphon Life turns that into healing. Blood Pact pays for spells with health when you're out of mana. |

- Holy Power and Souls show as pips under the cast bar.

- Trees: Priest has Holy, Discipline and Devotion; Druid has Restoration, Wild Spirit and Thornguard; Occultist has Affliction, Blood and Shadow.
- Talents are fewer and much bigger: up to 3 ranks of +5–15% per rank, plus keystones (2–3 points) that change how spells work. Examples: Chain Heal, Inner Light, Atonement, Divine Hymn, Lifebloom, Efflorescence, Germination, Tree of Life, Ironbark, Wrath, Soul Drain, Haunt, Vampiric Embrace, Curse of Doom and Eclipse of Souls. Each tree ends in a capstone.
- Defensive capstones: the Priest's **Retribution Ward** throws 40% of what a Ward absorbs back at the enemy, the Druid's **Blooming Bark** turns an ending Barkskin into a heal over time worth 20% of the target's health, and the Occultist's **Shattering Bones** makes a breaking Bone Shield hit every enemy for 60% of its absorb.
- **Tooltips.** Hover any talent (yours or a companion's) to see what it does, your rank, the cost and why it's locked if it is. Hovering a spell on the action bar shows its description, cost, cast time and cooldown, and hovering an item in the Armory shows its stats compared with what's equipped.
- Talents with a small spell icon need that spell and open once you know it. Deeper rows need points spent in that tree first (2 per row). Resetting is free.
- Talent points: 1 every 2 Cleric levels, plus 1 for each first dungeon clear, the Library and an achievement.
- Each class has its own spell icon colors, heal effects and casting sparkles. The Talents tab lists your spells as that class under "Your spells as a …".
- Party frames show one badge per heal over time with its class name and a stack count, for example "Rejuvenation ×3", Regrowth, Wild Growth, Leech Seed or Divine Hymn, plus Barkskin and Bone Shield. Enemies with Leech Seed show a red pip.
- Your weapon in the arena takes on its item's rarity: rare weapons glow blue, epic ones purple and legendary ones gold, pulsing. Epic or legendary armor still gives a colored outline.
- Numbers on the party frames rise from above the frame's right side so they don't cover the health text.
- Combat numbers are whole and bold. Heal-over-time and damage ticks that land close together on the same hero merge into one rising number instead of a pile.

## The party

- **Bram is the tank.** Enemies attack him about two thirds of the time (bosses always do). If he falls, the enemies run wild: they hit everyone 60% harder and 25% faster until the stage ends, with a red warning in the arena. His Bulwark tree has three new tank talents: **Guardian** (takes up to 24% of the damage aimed at other allies), **Challenging Shout** (enemies attack him more often) and **Unbreakable** (the rest of the party takes 10% less damage while he stands).
- **Party auras.** Each companion unlocks an aura at level 10 and doubles it at level 20: Bram's Guardian Aura (party takes 4% / 8% less damage), Rook's Battle Shout (+6% / +12% party damage), Vess's Hunter's Mark (enemies take 5% / 10% more damage) and Ilda's Arcane Intellect (+8% / +16% max mana). They're shown in the Party tab.

- **Gear baseline.** Every hero gets damage and health from the party's average item level, so a companion missing a weapon or wearing an old one falls behind a little instead of dropping to almost nothing. Your healer, who wears no companion gear, gets a stronger baseline and also gains health from promotions, so you sit around a caster's health rather than being one-shot.
- **Balanced damage.** Rook, Vess and Ilda now land within a few points of each other depending on spec and stage (about 22–38% of the party's damage each), with Bram around 6–18% as the tank. Ilda's area damage (Flamestrike, Pyroblast, Inferno, Arcane Surge, Meteor Storm) was toned down, Rook hits harder (and Whirlwind, Mortal Strike, Rampage and Brutality improved), and Vess's poison spreads less.
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
  | You (Priest) | Devout | Halo | Guardian Angel | Radiance (Heal also heals the next most injured) | Divine Favor | Ascension (Heal and Prayer +20%, −30% cost) |
  | You (Druid) | Attuned | Clearcasting | Nature's Guardian | Lifebinder (Regrowth also plants Rejuvenation) | Nature's Focus | Ancient of Lore (Regrowth and Rejuvenation +20%, −30% cost) |
  | You (Occultist) | Dread Pact | Dark Bargain | Soul Anchor | Hungering Drain (Drain Life splashes 25%) | Malice | Lich Form (Drain Life +20%, −30% cost) |

  Every hero starts scrappy and gears up in four steps, each with new pixel art, not just new colors:

  | Hero | Recruit | Veteran–Elite | Champion–Hero | Legend–Paragon |
  |---|---|---|---|---|
  | Bram | Padded jerkin, plank shield | Nasal helm, chainmail, kite shield | Plumed great helm, plate, tower shield | Winged gold helm with a glowing visor, gilded plate |
  | Rook | Torn shirt, rusty hatchet | Headband, leather, battle axe | Steel helm, mail and surcoat, double axe | Horned black plate, burning axe |
  | Vess | Peasant hood, stick bow | Green hood, leather, longbow | Ranger mantle, bracers, gilded recurve | Silver scale, feathered hood, moonlit bow |
  | Ilda | Patched robe, twig wand | Pointed hat, robe, staff | Banded hat, trimmed robe, orb staff | Starry arch-mage robe, crystal staff |
  | You (Priest) | Novice's robe and staff | White robe, gold stole | Mitre and vestments, sun staff | Halo, gilded vestments, radiant staff |
  | You (Druid) | Hide tunic, sapling | Leaf circlet, green robe | Antlers, bark pauldrons | Blossoming antlers, leaf cloak |
  | You (Occultist) | Rags and a bone charm | Dark hood, skull staff | Horned bone mask, bone pauldrons | Bone crown, rune robes, skull lantern |

  The second rank of each pair adds a cape (Elite) or a shining gem (Hero), and Paragon adds feathered wings of light. Reaching a new gear step gets a bigger flash and a "New gear!" toast. Colored rank pips sit over each hero in combat. The Party tab shows a portrait for every rank, a before-and-after preview of the next promotion and the full perk list.

## Other progression

- **Gear.** Enemies drop items for the Cleric's six slots and the companions' three, in five rarities. The header shows your **party item level**, the average across all 18 slots. **Equip best items** fills every slot automatically: armor goes to the tank first, and weapons and charms go to the hardest hitters first. Enchant equipped items with gold for +10% stats per level.
- **Item sets.** Each companion and the Cleric has a three-piece set that sometimes drops in place of a rare-or-better item (set pieces are always epic, with teal names). Two pieces give a stat bonus, and three unlock a synergy: Bram's hits sunder armor, Rook always crits slowed or stunned enemies, Vess's crits mark enemies for 8 seconds, Ilda's fireballs chill, and the Cleric's heals on low allies also shield them. The item view shows the set's pieces and bonuses.
- **Looks.** Promotions show on the battlefield as new armor and weapons (see the table above), with a glowing aura and rising motes from Hero. Epic or legendary armor gives a colored outline and trims the torso in its rarity color, legendary armor adds a pulsing gem on the chest, and an epic or legendary helmet puts a circlet on your Cleric. Weapons glow in their rarity color, and epic or legendary ones sparkle.
- **Loot filter.** In the Armory, choose to auto-sell drops below a rarity (upgrades are never sold), and optionally equip upgrades as they drop. When the bag is full, the weakest non-upgrade is sold to make room, and a **Bag full** warning appears (as a toast, at most once a minute, and as a tag in the arena header). The Armory tab shows a dot when the bag is full or holds an upgrade.
- **Gear warnings.** Each party frame shows **▲ Upgrade** when the bag holds something better for that hero (click it to equip the best items) and **⚠ Old gear** when a slot is empty or well below the item level of your deepest dungeon (click it to open the Armory).
- **Merchant.** Once you build a Market, the Armory sells sealed items for the deepest dungeon you've reached: a Supply Crate (any rarity), a Gilded Coffer (rare or better) and a Royal Reliquary (epic or better, 20% legendary).
- **Elixirs.** As the Herb Garden grows, the Dungeons tab sells three elixirs (+25% party damage, 15% less damage taken, +40% mana regeneration). Each lasts 10 minutes of fighting and stacks up to an hour. Their price scales with your deepest dungeon.
- **Achievements.** Fifteen achievements, such as clearing a dungeon without a death, slaying ten elites, wearing a full set or clearing at Peril 3. Each grants a small permanent bonus: healing, damage, gold, experience, mana or a talent point. They're listed in the Chronicle with progress bars.
- **Chronicle.** Healing by spell for this run or all time, with share, overheal and casts, plus damage taken, party deaths, damage absorbed by shields and deaths per dungeon.
- **Combat timeline.** The end-of-run screen and the Chronicle draw your last run as a graph: damage taken (red), effective healing (green) and overheal (dashed), with a line where each hero died (and who killed them), a ▼ for each boss ability and markers for each stage and the boss. Hover the markers for details. Use it to see where the damage spiked and whether your healing kept up.
- **Crafting with materials.** The Smithy turns materials into gear upgrades. Every item uses the materials of the dungeon its item level comes from:
  - **Salvage** (Smithy 1): break a bag item into materials.
  - **Empower** (Smithy 1): raise an item one rarity, up to Legendary. Its stats grow and it gains new ones.
  - **Imbue** (Smithy 4): add one extra stat to an item, once.
  - **Masterwork** (Smithy 8): crafting costs 30% fewer materials.
- **Day and night.** The world runs on a 12-minute day. By day, kills pay **+15% gold**; at night, stages give **+15% experience and materials**. The arena header and the Town show which it is and how long until it turns. The Town shows a blue sky and sun by day, a warm dusk and dawn, and a starry night with a moon, lit windows and lamps, fireflies and fewer villagers out.
- **Prosperity.** Every Town building level adds to your Prosperity, and milestones grant permanent bonuses:

  | Levels | Title | Bonus |
  |---|---|---|
  | 5 | Hamlet | +5% gold find |
  | 12 | Village | **Tithes**: the town collects gold for you every 2 hours (up to 2 stored) |
  | 20 | Market Town | +10% experience |
  | 30 | Town | a fourth bounty, and banners on the main street |
  | 42 | City | day and night bonuses doubled |
  | 56 | Great City | one more mana potion per run, +10% gold find |
  | 72 | Capital | expeditions last up to 12 hours, and festival lights over the street |
  | 90 | Jewel of the Realm | +20% party damage and a golden fountain |

  **The town flourishes as it grows.** More villagers come out with every building and level (some walk the chapel lane, some carry baskets, wear hats or are children), up to a crowd of nearly thirty. New sights appear as Prosperity rises: flower beds along the lane (2), chickens (5), a washing line (8), market stalls with merchants (12), wheat fields with a scarecrow and a farmer (16), a merchant cart that rolls down the main street (20), ducks on the pond (25), banners, bunting and a third stall (30), a bard at the fountain (36), children playing around the plaza (42), the city watch on patrol (50), a hot-air balloon (56), blossom drifting from the orchard (64), festival lights and fireworks at night (72), sky lanterns rising at night (80), and a golden fountain with a rainbow in its spray (90). The Prosperity panel lists how many sights you've unlocked and what's next. In any town, cloud shadows drift over the grass, sun shafts fall across it by day and the pond shimmers.
- **Bounty Board.** The Town shows three bounties at a time, such as "Defeat 40 enemies in the Cinder Pit", "Defeat 4 elites", "Save 4 allies who are below 10% health", "Clear 5 stages without anyone falling" or "Clear the Hollow Crypt as an Occultist". Finished bounties pay gold and materials, and one in five also gives an epic item. Reroll one you don't like for gold. The Town tab shows a dot when one is ready to claim.
- **Item mastery.** Every item teaches a skill. Clear stages with it equipped to master it, and the skill is yours for good.
- **The Town.** Every stage drops materials from its dungeon (Rat Tails, Bog Moss and so on), with more at high Devotion. The Town tab shows your town as a pixel-art map with eight plots. Click a plot to see what it would do, and build it: the building rises out of the ground and stays on the map, gaining a banner at level 4 and gold trim at level 8. Buildings go up to level 12 and cost gold plus materials. Level 1 uses materials from the first dungeon, level 2 from the second, and so on, so pushing deeper (including Act II) unlocks the next tier:

  | Building | Every level | Unlocks |
  |---|---|---|
  | Acolyte Cloister | A stronger Acolyte and faster expeditions | Lv 3 the Acolyte lays a heal over time on the most injured ally every 8 seconds · Lv 5 the Acolyte shields Bram |
  | Infirmary | Better resting; fallen allies return with more health | Lv 3 Triage: allies below 25% take less damage · Lv 6 Second Wind: once per stage the first ally to fall gets back up |
  | Herb Garden | One more mana potion per run | Lv 2/4/6 the three elixirs · Lv 3 Healing Draught (heals the party for 25%, on F) · Lv 7 a second draught |
  | Chapel | Start with Devotion; Devotion fades slower | Lv 3 Chapel Bell (+35 Devotion once per run, on R) · Lv 6 Devotion never falls below 20% |
  | Library | More experience | Lv 3 and 7 a bonus Cleric talent point · Lv 5 first clears offer four spells |
  | Smithy | Cheaper, stronger enchanting | Lv 1 Salvage and Empower · Lv 3 Reforge (reroll an item's stats) · Lv 4 Imbue · Lv 5 every drop is one item level higher · Lv 8 Masterwork |
  | Barracks | Cheaper promotions | Lv 2 Battle Stances (Aggressive, Balanced or Defensive, in the Party tab) · Lv 4 +20% experience |
  | Market | Cheaper sealed items | Lv 1/3/5 Supply Crates, Gilded Coffers and Royal Reliquaries |

  Click a building on the map (anywhere on it, including its annex) or pick it from the building bar under the map to see its milestones, with what's unlocked and what comes next.

  The Town tab also sells one-time blessings for gold.
- **Expeditions.** Once you build the Acolyte Cloister, an Acolyte heals the party in the background (weakly at first). While the game is closed or in another tab, the Acolyte leads the party through the dungeon you're in, if you've cleared it, otherwise your deepest clear. They run at 20–55% of your active pace for up to 8 hours and bring back gold, experience, materials and items.
- **While you were away.** When you come back, a summary shows how long you were gone, which dungeon your Acolyte farmed and roughly how many times, and what they brought: gold, experience, materials, any tithes ready to collect, and items (the best six shown, with upgrades marked). Nothing is added until you press **Claim all**, which also levels up the party and, if you turned it on, equips upgrades. Without the Cloister or a cleared dungeon, the summary tells you what to do first.

## Interface

- Buttons press in when clicked, cards lift on hover, the tab underline slides and each tab fades in, toasts and pop-ups animate in, gold pops when it goes up, and spells flash on the action bar when used. Scrollbars, section headers, records, the battle log and the save panel were restyled to match.

## Save codes

- The Chronicle tab can **export a save code**: your whole save, compressed into a short block of text. Copy it, and later **import** it in any browser to continue from there. Importing replaces your current progress.

## Playtesting

- **Quickest:** open `index.html` straight from disk by double-clicking it.
- **Local server:** `python3 -m http.server 8000` in this folder, then open <http://localhost:8000>.
- **Playtest tools:** add `#dev` to the end of the address (for example `index.html#dev`) to show a panel under the spell bar: game speed 1× / 3× / 10×, +1K gold, gold ×10, +5 Cleric talent points, +20 materials, simulate 1 hour away, win the current stage, unlock the next dungeon, drop an item, level everyone up, and infinite mana. Remove `#dev` to hide it again.
- **Fresh start:** Chronicle tab → *Start over*, or use a private window.
- **On your phone or for friends:** turn on GitHub Pages (repo Settings → Pages → *Deploy from a branch*, pick the branch and `/ (root)`).
