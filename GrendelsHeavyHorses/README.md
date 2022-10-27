Purpose
Expand on horses

#Things that have happened already

1. Add draught horses and have them spawn at farms - 1x chance 30 per farm Size for draught horses based on a Shire Horse stallion: 

Size 1000kg, average top speed 35MPH, roughly same as a Standardbred

Changes: 550 kg to 1000 kg, volume 550k to 1000k, carry ratio from 20% to 25%

Google suggests, among others, that "The average top speed of a horse is 25 to 30 mph," implying some draught horses can be faster than average

#Things that will probably never happen

2. Training regimen for regular horses and draught horses into the appropriate war horse type

3. Expanded war horse behaviour: assisting in combat, going home, coming when whistled for

#Addendum on tilesets not showing ridden draught horses

Issue: while riding, your character looks like they are behind the horse

Steps to fix: 

1. go into gfx/[your_tileset_here]/tile_config.json
2. search for rid_mon_horse
3. Whatever that line says, duplicate it and change above phrase into rid_mon_horse_draught for the duplicated line

Examples

So eg in MSX++UnDeadPeopleEdition you will find

{"id": "rid_mon_horse", "fg": 18429, "rotates": false},

and add 

{"id": "rid_mon_horse_draught", "fg": 18429, "rotates": false},

or, in UltimateCataclysm, you will find

{ "id": "rid_mon_horse", "fg": [ { "weight": 1, "sprite": 8869 }, { "weight": 1, "sprite": 8870 } ] },

and add

{ "id": "rid_mon_horse_draught", "fg": [ { "weight": 1, "sprite": 8869 }, { "weight": 1, "sprite": 8870 } ] },
