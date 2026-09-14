# elementalis

Elementalis — Update

Visuals

Every element now has its own projectile art, flight trail and impact effect. Previously all 21 shared one glowing diamond with the colour swapped — fire now throws burning darts that shed soot, water is a foam-lipped crescent that splashes, obsidian is black glass with a burning edge that shatters into falling splinters, arcane is a sigil inside a counter-rotating ring.
18 distinct particle textures replace the single glow sprite used for everything: embers, water droplets, ice crystals, rock chips, leaves, bone, glass, ash, sigils, wisps, smoke and sparkles.
Ground effects are drawn as what they are — lava pools crust over with glowing cracks, vines visibly grow outward, the void rift reads as an actual hole, steam billows.
Enemies carry physical elemental features (flame crowns, dripping veils, bolted rock slabs, wind curls, orbiting sigils) instead of just being tinted.
Each element has its own icon in the spell bar and Grimoire.
Added critical hits, and rebalanced screen shake and flashes — small hits got more punch, the big spells got toned down so they no longer white out the screen.

Sound — all new. Fully procedural, no audio files: a distinct cast voice per element family plus hit, kill, hurt, blink, level-up and fusion sounds. Toggle in the top right.

Gameplay

Enemies now telegraph their attacks with a wind-up ring, so ranged shots and boss attacks can be read and dodged.
Wardens have less health (520 → 450) and mana regenerates a little faster.
Fusions are easier to reach — lower mastery requirements and essence costs, so the third-circle elements and Ascendant are attainable in a normal run.
Clearing an enemy camp now pays an essence bonus.
The compass points to the nearest shrine of an element you haven't attuned yet, rather than just the nearest shrine.

World generation

The world is now randomly seeded — previously every playthrough generated the identical map, shrines and starting position.
Shrine elements are evenly distributed. They used to be tied to biome, which made Earth shrines overwhelmingly common and Fire and Arcane rare.
Shrines are guaranteed to be spaced apart instead of sometimes spawning almost on top of each other.
Your starting position varies between runs.

Fixes

Fixed a hash overflow that was skewing terrain and site generation.
Boss attacks no longer continue firing while the Grimoire is open or after you die.
Holding Shift no longer chain-dashes.
The death screen no longer stacks on top of the Grimoire.
Fixed garbled characters appearing in on-screen messages.
Fixed the HUD not updating live — the mana bar now visibly refills, and mastery levels and the selected-slot highlight update immediately.

Performance

Terrain generation is spread across frames, removing the stutter when moving into new areas (a ~12ms spike per chunk down to ~3ms).
Faster particle handling, cached gradients, and reduced per-frame work throughout.
Quality scaling under load now only thins background ambience — spell effects, enemies and lighting are never reduced.
