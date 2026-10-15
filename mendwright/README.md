# Mendwright

A small healing game in a single HTML file, in the spirit of Mini Healer, with gear drops and Cookie Clicker–style idle progression.

Open `index.html` in a browser. Progress saves to your browser's local storage every 10 seconds.

## How to play

- **Heal the party.** Click a party frame to target it, then click a spell or press `1`–`5`. Hovering a frame and pressing a key casts on that frame. `Esc` cancels a cast.
- **Spells:** Mend (slow, efficient), Flash Heal (fast, costly), Renew (heal over time, stage 2), Ward (absorb shield, stage 4), Prayer (heals everyone, stage 6).
- **Bosses** auto-attack the tank and cast telegraphed abilities (Cleave, Searing Wave, Shadow Bolt, Festering Bite, Frenzy). They enrage below 20% health and go berserk after 2 minutes.
- **You lose** if you die or the rest of the party dies. Beat the boss to unlock the next stage, or step back to farm gear.

## Progression

- **Healing earns gold.** Overhealing earns nothing.
- **Sanctum:** buildings that earn gold every second, with costs that grow ×1.15 per purchase. Blessings are one-time upgrades: building multipliers, more gold from healing, mana regen, better loot and more.
- **Barracks:** party training for damage, max health and passive regeneration.
- **Armory:** every boss drops gear for one of six slots (Head, Chest, Hands, Staff, Ring, Trinket). Items come in five rarities and roll stats: Spell Power, Max Mana, Mana Regen, Critical, Haste, Gold Find and Party Vigor. Equipped items can be enchanted with gold for +10% stats per level.
- **Offline earnings:** buildings keep earning while you're away, for up to 8 hours.
