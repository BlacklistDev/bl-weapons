# bl-weapons
* If you still have issues please put them in the Issues tab, im still working on this, but they work for me and everyway I use them

## Installation ##

-- Put the weapons file in your resources folder
## Drop this code in ``qb-weapons/server/main.lua line 303``
````
QBCore.Functions.CreateUseableItem('flame_ammo', function(source, item)
    TriggerClientEvent('weapons:client:AddAmmo', source, 'AMMO_FLAME', 500, item)
end)

QBCore.Functions.CreateUseableItem('nail_ammo', function(source, item)
    TriggerClientEvent('weapons:client:AddAmmo', source, 'AMMO_NAIL', 20, item)
end)

QBCore.Functions.CreateUseableItem('taser_ammo', function(source, item)
    TriggerClientEvent('weapons:client:AddAmmo', source, 'AMMO_TASER', 1, item)
end)

QBCore.Functions.CreateUseableItem('paintball_ammo', function(source, item)
    TriggerClientEvent('weapons:client:AddAmmo', source, 'AMMO_PAINTBALL', 20, item)
end)

QBCore.Functions.CreateUseableItem('ltl_ammo', function(source, item)
    TriggerClientEvent('weapons:client:AddAmmo', source, 'AMMO_LTL', 10, item)
end)

````
## Drop this code in ``qb-core/shared/items.lua``
```lua
--Blacklist Custom WEAPONS
['weapon_flamethrower']                   = {['name'] = 'weapon_flamethrower',                     ['label'] = 'Flamethrower',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_FLAME',              ['image'] = 'weapon_flamethrower.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['flame_ammo']                   = {['name'] = 'flame_ammo',                     ['label'] = 'Flamethrower Fuel',               ['weight'] = 1000,         ['type'] = 'item',     ['ammotype'] = nil,              ['image'] = 'flame_ammo.png',             ['unique'] = false,         ['useable'] = false,    ['combinable'] = nil,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['nail_ammo']                   = {['name'] = 'nail_ammo',                     ['label'] = 'Nails',               ['weight'] = 1000,         ['type'] = 'item',     ['ammotype'] = nil,              ['image'] = 'nail_ammo.png',             ['unique'] = false,         ['useable'] = false,    ['combinable'] = nil,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['ltl_ammo']                   = {['name'] = 'ltl_ammo',                     ['label'] = 'Slug Ammo',               ['weight'] = 1000,         ['type'] = 'item',     ['ammotype'] = nil,              ['image'] = 'slug_ammo.png',             ['unique'] = false,         ['useable'] = false,    ['combinable'] = nil,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['paintball_ammo']                   = {['name'] = 'paintball_ammo',                     ['label'] = 'Paintball Pod',               ['weight'] = 1000,         ['type'] = 'item',     ['ammotype'] = nil,              ['image'] = 'paintball_ammo.png',             ['unique'] = false,         ['useable'] = false,  ['combinable'] = nil,   ['description'] = 'A small firearm designed to be held in one hand'},
    ['taser_ammo']                   = {['name'] = 'taser_ammo',                     ['label'] = 'Taser Ammo',               ['weight'] = 1000,         ['type'] = 'item',     ['ammotype'] = nil,              ['image'] = 'taser_ammo.png',             ['unique'] = false,         ['useable'] = false,   ['combinable'] = nil,  ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_taser']                   = {['name'] = 'weapon_taser',                     ['label'] = 'Taser',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_TASER',              ['image'] = 'weapon_stungun.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_dp9']                   = {['name'] = 'weapon_dp9',                     ['label'] = 'Diamondback 9',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_PISTOL',              ['image'] = 'weapon_dp9.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_ltl']                   = {['name'] = 'weapon_ltl',                     ['label'] = 'Bean Bag Shotgun',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_SHOTGUN',              ['image'] = 'weapon_ltl.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_staff']                   = {['name'] = 'weapon_staff',                     ['label'] = 'Staff',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'staff.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_sledgehammer']                   = {['name'] = 'weapon_sledgehammer',                     ['label'] = 'Sledge Hammer',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'weapon_sledgehammer.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_karambit']                   = {['name'] = 'weapon_karambit',                     ['label'] = 'Karambit',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'weapon_karambit.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_dagger']                   = {['name'] = 'weapon_dagger',                     ['label'] = 'Dagger',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'weapon_dagger.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_shoe']                   = {['name'] = 'weapon_shoe',                     ['label'] = 'Shoe',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'shoe.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_brick']                   = {['name'] = 'weapon_brick',                     ['label'] = 'Brick',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'brick.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_book']                   = {['name'] = 'weapon_book',                     ['label'] = 'Book',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'book.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_keyboard']                   = {['name'] = 'weapon_keyboard',                     ['label'] = 'Keyboard',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'keyboard.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_katanas']                   = {['name'] = 'weapon_katanas',                     ['label'] = 'Katana',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'katana.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_katana']                   = {['name'] = 'weapon_katana',                     ['label'] = 'Light Saber',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = nil,              ['image'] = 'katanas.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_draco']                   = {['name'] = 'weapon_draco',                     ['label'] = 'Draco',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_pistol.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_gepard']                   = {['name'] = 'weapon_gepard',                     ['label'] = 'Gepard',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_gepard.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_groza']                   = {['name'] = 'weapon_groza',                     ['label'] = 'Groza',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_groza.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_scar']                   = {['name'] = 'weapon_scar',                     ['label'] = 'Scar',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_scar.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_bolt']                   = {['name'] = 'weapon_bolt',                     ['label'] = 'Bolt',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_blot.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_1911']                   = {['name'] = 'weapon_1911',                     ['label'] = '1911',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_PISTOL',              ['image'] = 'weapon_browning.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_browning']                   = {['name'] = 'weapon_browning',                     ['label'] = 'Browning',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_PISTOL',              ['image'] = 'weapon_glock.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_g18c']                   = {['name'] = 'weapon_g18c',                     ['label'] = 'Glock 18 C',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_PISTOL',              ['image'] = 'weapon_glock17.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_mp5']                   = {['name'] = 'weapon_mp5',                     ['label'] = 'MP 5',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_mp5.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_dragunov']                   = {['name'] = 'weapon_dragunov',                     ['label'] = 'Dragunov',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_dragunov.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_g22']                   = {['name'] = 'weapon_g22',                     ['label'] = 'Glock 22',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_PISTOL',              ['image'] = 'weapon_sniperrifle.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_m14']                   = {['name'] = 'weapon_m14',                     ['label'] = 'M-14',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_m14.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_m24']                   = {['name'] = 'weapon_m24',                     ['label'] = 'M-24',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_m24.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_nailgun']                   = {['name'] = 'weapon_nailgun',                     ['label'] = 'Nail Gun',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_nailgun.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_m4']                   = {['name'] = 'weapon_m4',                     ['label'] = 'M-4',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_RIFLE',              ['image'] = 'weapon_m4.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_glock']                   = {['name'] = 'weapon_glock',                     ['label'] = 'Glock',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_PISTOL',              ['image'] = 'weapon_glock.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},
    ['weapon_uzi']                   = {['name'] = 'weapon_uzi',                     ['label'] = 'Uzi',               ['weight'] = 1000,         ['type'] = 'weapon',     ['ammotype'] = 'AMMO_SMG',              ['image'] = 'weapon_uzi.png',             ['unique'] = true,         ['useable'] = false,     ['description'] = 'A small firearm designed to be held in one hand'},

  
```
## Drop The Next code in qb-core/shared/weapons.lua ##
```lua
-- Blacklist Custom Weapons
	[`weapon_nailgun`] 		 			= {['name'] = 'weapon_nailgun', 	 				['label'] = 'Nail Gun', 			['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_NAIL',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_flamethrower`] 		 			= {['name'] = 'weapon_flamethrower', 	 				['label'] = 'Flamethrower', 			['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_FLAME',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_m4`] 		 			= {['name'] = 'weapon_m4', 	 				['label'] = 'M4A1 Carbine', 			['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_dragunov`] 		 = {['name'] = 'weapon_dragunov', 	 	['label'] = 'Dragunov', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_draco`] 		 = {['name'] = 'weapon_draco', 	 	['label'] = 'Draco', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_gepard`] 		 = {['name'] = 'weapon_gepard', 	 	['label'] = 'Gepard', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_groza`] 		 = {['name'] = 'weapon_groza', 	 	['label'] = 'Groza', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_scar`] 		 = {['name'] = 'weapon_scar', 	 	['label'] = 'Scar', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_m24`] 		 = {['name'] = 'weapon_m24', 	 	['label'] = 'M24', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_m14`] 		 = {['name'] = 'weapon_m14', 	 	['label'] = 'M14', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_taser`] 		 = {['name'] = 'weapon_taser', 	 	['label'] = 'Taser', 				['ammotype'] = 'AMMO_TASER',	['damagereason'] = 'Taserd in the ass'},
	[`weapon_skorpion`] 		 = {['name'] = 'weapon_skorpion', 	 	['label'] = 'Skorpion', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_ltl`] 		 = {['name'] = 'weapon_ltl', 	 	['label'] = 'PD Bean Bag Shotgun', 				['ammotype'] = 'AMMO_LTL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_mp5`] 		 = {['name'] = 'weapon_mp5', 	 	['label'] = 'Dragunov', 				['ammotype'] = 'AMMO_SMG',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_g18`] 		 = {['name'] = 'weapon_g18', 	 	['label'] = 'Glock 18', 				['ammotype'] = 'AMMO_PISTOL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_g18c`] 		 = {['name'] = 'weapon_g18c', 	 	['label'] = 'Glock 18C', 				['ammotype'] = 'AMMO_PISTOL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_dp9`] 		 = {['name'] = 'weapon_dp9', 	 	['label'] = 'PD DP9', 				['ammotype'] = 'AMMO_PISTOL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_browning`] 		 = {['name'] = 'weapon_browning', 	 	['label'] = 'Glock 18', 				['ammotype'] = 'AMMO_PISTOL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_1911`] 		 = {['name'] = 'weapon_1911', 	 	['label'] = 'Glock 18', 				['ammotype'] = 'AMMO_PISTOL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_potatolauncher`] 		 = {['name'] = 'weapon_potatolauncher', 	 	['label'] = 'Potato Launcher', 				['ammotype'] = 'AMMO_PISTOL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_staff`] 		 = {['name'] = 'weapon_dragunov', 	 	['label'] = 'Staff', 				['ammotype'] = 'AMMO_PISTOL',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_gavel`] 				 = {['name'] = 'weapon_gavel', 		['label'] = 'Gavel', 		['weapontype'] = 'Melee',	['ammotype'] = nil,	['damagereason'] = 'Knifed / Stabbed / Eviscerated'},
	[`weapon_flamethrower`] 				 = {['name'] = 'weapon_flamethrower', 		['label'] = 'Flamethrower', 		['ammotype'] = nil,	['damagereason'] = 'Knifed / Stabbed / Eviscerated'},
	[`weapon_katana`] 			 	= {['name'] = 'weapon_katana', 				['label'] = 'Katana', 					['weapontype'] = 'Melee',			['ammotype'] = nil,						['damagereason'] = 'Knifed / Stabbed / Eviscerated'},
	[`weapon_shiv`] 			 	= {['name'] = 'weapon_shiv', 				['label'] = 'Shiv', 					['weapontype'] = 'Melee',			['ammotype'] = nil,						['damagereason'] = 'Knifed / Stabbed / Eviscerated'},
	[`weapon_sledgehammer`] 		= {['name'] = 'weapon_sledgehammer', 		['label'] = 'Sledge Hammer', 			['weapontype'] = 'Melee',			['ammotype'] = nil,						['damagereason'] = 'Melee killed / Whacked / Executed / Beat down / Murdered / Battered'},
	[`weapon_karambit`] 			= {['name'] = 'weapon_karambit', 			['label'] = 'Karambit', 				['weapontype'] = 'Melee',			['ammotype'] = nil,						['damagereason'] = 'Knifed / Stabbed / Eviscerated'},
	[`weapon_keyboard`] 			= {['name'] = 'weapon_keyboard', 			['label'] = 'Keyboard', 				['weapontype'] = 'Melee',			['ammotype'] = nil,						['damagereason'] = 'Melee killed / Whacked / Executed / Beat down / Murdered / Battered'},
	[`weapon_glock17`] 		 		= {['name'] = 'weapon_glock17', 			['label'] = 'Glock-17',		    		['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_glock`] 		 	= {['name'] = 'weapon_glock', 					['label'] = 'Glock',		    		['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_glock22`] 		 		= {['name'] = 'weapon_glock22', 			['label'] = 'Glock-22',		    		['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_deagle`] 		 		= {['name'] = 'weapon_deagle', 				['label'] = 'Desert Eagle',		    	['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_fnx45`] 		 		= {['name'] = 'weapon_fnx45', 				['label'] = 'FN FNX-45',		    	['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_m1911`] 		 		= {['name'] = 'weapon_m1911', 				['label'] = 'M1911',		    		['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_glock20`] 		 		= {['name'] = 'weapon_glock20', 			['label'] = 'Glock-20',		    		['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_glock19gen4`] 		 	= {['name'] = 'weapon_glock19gen4', 		['label'] = 'Glock-19 Gen 4',		    ['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
	[`weapon_pmxfm`] 			 	= {['name'] = 'weapon_pmxfm', 				['label'] = 'Beretta PMX', 				['weapontype'] = 'Submachine Gun',	['ammotype'] = 'AMMO_SMG',				['damagereason'] = 'Riddled / Drilled / Finished / Submachine Gunned'},
	[`weapon_mac10`] 			 	= {['name'] = 'weapon_mac10', 				['label'] = 'MAC-10', 					['weapontype'] = 'Submachine Gun',	['ammotype'] = 'AMMO_SMG',				['damagereason'] = 'Riddled / Drilled / Finished / Submachine Gunned'},
	[`weapon_mk47fm`] 		 		= {['name'] = 'weapon_mk47fm', 	 			['label'] = 'MK47 Mutant', 				['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_m6ic`] 		 		= {['name'] = 'weapon_m6ic', 	 			['label'] = 'LWRC M6IC', 				['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_scarsc`] 		 		= {['name'] = 'weapon_scarsc', 	 			['label'] = 'Scar SC', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_ak47`] 		 		= {['name'] = 'weapon_ak47', 	 			['label'] = 'AK-47', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_ak74`] 		 		= {['name'] = 'weapon_ak74', 	 			['label'] = 'AK-74', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_aks74`] 		 		= {['name'] = 'weapon_aks74', 	 			['label'] = 'AKS-74', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_groza`] 		 		= {['name'] = 'weapon_groza', 	 			['label'] = 'OTs-14 Groza', 			['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_scarh`] 		 		= {['name'] = 'weapon_scarh', 	 			['label'] = 'Scar-H', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
```
## Drop The Next Code in ``qb-weapons/config.lua``
```lua
-- Blacklist Custom Weapons
    ['weapon_ak47'] 			= 0.15,
    ['weapon_de'] 	                = 0.15,
    ['weapon_fnx45'] 			= 0.15,
    ['weapon_glock17'] 		        = 0.15,
    ['weapon_m4'] 			= 0.15,
    ['weapon_hk416'] 			= 0.15,
    ['weapon_mk14'] 			= 0.15,
    ['weapon_m110'] 			= 0.15,
    ['weapon_huntingrifle'] 	        = 0.20,
    ['weapon_ar15'] 			= 0.15,
    ['weapon_m9'] 	                = 0.15,
    ['weapon_m70'] 			= 0.15,
    ['weapon_m1911'] 		        = 0.15,
    ['weapon_mac10'] 			= 0.15,
    ['weapon_uzi'] 	                = 0.15,
    ['weapon_mp9'] 	                = 0.15,
    ['weapon_mossberg'] 		= 0.15,
    ['weapon_remington'] 		= 0.15,
    ['weapon_scarh'] 			= 0.15,
    ['weapon_shiv'] 	                = 0.15,
    ['weapon_katana'] 	                = 0.15,
    ['weapon_sledgehammer'] 	        = 0.15,
    ['weapon_mp5'] 			= 0.15,
    ['weapon_glock18c'] 		= 0.15,
    ['weapon_glock22'] 			= 0.15,
    ['weapon_aks74'] 			= 0.15,
    ['weapon_ak74'] 			= 0.15,
    ['weapon_dragunov'] 			= 0.15,
    ['weapon_draco'] 				= 0.15,
    ['weapon_gepard'] 				= 0.15,
    ['weapon_groza'] 				= 0.15,
    ['weapon_scar'] 				= 0.15,
    ['weapon_mpx'] 				    = 0.15,
    ['weapon_m24'] 				    = 0.15,
    ['weapon_m14'] 				    = 0.15,
    ['weapon_g22'] 				    = 0.15,
    ['weapon_skorpion'] 			= 0.15,
    ['weapon_ltl'] 				    = 0.15,
    ['weapon_izh81'] 				= 0.15,
    ['weapon_mp5'] 				    = 0.15,
    ['weapon_g18'] 				    = 0.15,
    ['weapon_g18c'] 				= 0.15,
    ['weapon_dp9'] 				    = 0.15,
    ['weapon_browning'] 			= 0.15,
    ['weapon_1911'] 				= 0.15,
    ['weapon_keyboard'] 			= 0.15,
    ['weapon_potatolauncher'] 		= 0.15,
    ['weapon_potato'] 				= 0.15,
    ['weapon_px'] 				    = 0.15,
    ['weapon_pi'] 				    = 0.15,
    ['weapon_staff'] 				= 0.15,
    ['weapon_bolt'] 				= 0.15,
```
## Drop the next code in ``qb-weapons/config.lua``
```lua
    ['WEAPON_M9'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_M9_CLIP_01',
            item = 'pistol_defaultclip',
            type = 'clip',
        },
        ['extendedclip'] = {
            component = 'COMPONENT_M9_CLIP_02',
            item = 'pistol_extendedclip',
            type = 'clip',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_PI_SUPP_02',
            item = 'pistol_suppressor',
        },
    },
    ['WEAPON_M1911'] = {
        ['suppressor'] = {
            component = 'COMPONENT_AT_PI_SUPP_02',
            item = 'pistol_suppressor',
        },
    },
    ['WEAPON_DE'] = {
        ['suppressor'] = {
            component = 'COMPONENT_AT_PI_SUPP_02',
            item = 'pistol_suppressor',
        },
    },
    ['WEAPON_FNX45'] = {
        ['suppressor'] = {
            component = 'COMPONENT_AT_PI_SUPP_02',
            item = 'pistol_suppressor',
        },
    },
    ['WEAPON_MP9'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_MP9_CLIP_01',
            item = 'microsmg_defaultclip',
            type = 'clip',
        },
        ['extendedclip'] = {
            component = 'COMPONENT_MP9_CLIP_02',
            item = 'microsmg_extendedclip',
            type = 'clip',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_AR_SUPP_02',
            item = 'pistol_suppressor',
        },
        ['scope'] = {
            component = 'COMPONENT_AT_SCOPE_MACRO',
            item = 'microsmg_scope',
        },
    },
    ['WEAPON_UZI'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_MICROSMG_CLIP_01',
            item = 'microsmg_defaultclip',
            type = 'clip',
        },
        ['extendedclip'] = {
            component = 'COMPONENT_MICROSMG_CLIP_02',
            item = 'microsmg_extendedclip',
            type = 'clip',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_AR_SUPP_02',
            item = 'pistol_suppressor',
        },
    },
    ['WEAPON_MAC10'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_MICROSMG_CLIP_01',
            item = 'microsmg_defaultclip',
            type = 'clip',
        },
        ['extendedclip'] = {
            component = 'COMPONENT_MICROSMG_CLIP_02',
            item = 'microsmg_extendedclip',
            type = 'clip',
        },
        ['flashlight'] = {
            component = 'COMPONENT_AT_PI_FLSH',
            item = 'pistol_flashlight',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_AR_SUPP_02',
            item = 'pistol_suppressor',
        },
    },
    ['WEAPON_AK47'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_AK47_CLIP_01',
            item = 'assaultrifle_defaultclip',
            type = 'clip',
        },
        ['extendedclip'] = {
            component = 'COMPONENT_AK47_CLIP_02',
            item = 'assaultrifle_extendedclip',
            type = 'clip',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_AR_SUPP_02',
            item = 'rifle_suppressor',
        },
    },
    ['WEAPON_M70'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_M70_CLIP_01',
            item = 'assaultrifle_defaultclip',
            type = 'clip',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_AR_SUPP_02',
            item = 'rifle_suppressor',
        },
    },
    ['WEAPON_M110'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_M110_CLIP_01',
            item = 'marksmanrifle_defaultclip',
            type = 'clip',
        },
        ['extendedclip'] = {
            component = 'COMPONENT_M110_CLIP_02',
            item = 'marksmanrifle_extendedclip',
            type = 'clip',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_AR_SUPP',
            item = 'rifle_suppressor',
        },
    },
    ['WEAPON_HK416'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_HK416_CLIP_01',
            item = 'carbinerifle_defaultclip',
            type = 'clip',
        },
        ['extendedclip'] = {
            component = 'COMPONENT_HK416_CLIP_02',
            item = 'carbinerifle_extendedclip',
            type = 'clip',
        },
        ['flashlight'] = {
            component = 'COMPONENT_AT_AR_FLSH',
            item = 'rifle_flashlight',
        },
        ['suppressor'] = {
            component = 'COMPONENT_AT_AR_SUPP',
            item = 'rifle_suppressor',
        },
    },
```
## Add the next code in ``qb-smallresources/client/weapondraw.lua``
```lua
    'WEAPON_DRAGUNOV',
    'WEAPON_DRACO',
    'WEAPON_GEPARD',
    'WEAPON_GROZA',
    'WEAPON_SCAR',
    'WEAPON_MPX',
    'WEAPON_M24',
    'WEAPON_M14',
    'WEAPON_G22',
    'WEAPON_SKORPION',
    'WEAPON_LTL',
    'WEAPON_MP5',
    'WEAPON_G18',
    'WEAPON_G18C',
    'WEAPON_DP9',
    'WEAPON_BROWNING',
    'WEAPON_1911',
    'WEAPON_POTATOLAUNCHER',
    'WEAPON_STAFF',
    'WEAPON_FLAMETHROWER',
    'WEAPON_KATANA',
    'WEAPON_SHIV',
    'WEAPON_SLEDGEHAMMER',
    'WEAPON_KARAMBIT',
    'WEAPON_KEYBOARD',
    'WEAPON_GLOCK17',
    'WEAPON_GLOCK18C',
    'WEAPON_GLOCK22',
    'WEAPON_DEAGLE',
    'WEAPON_FNX45',
    'WEAPON_M1911',
    'WEAPON_GLOCK20',
    'WEAPON_GLOCK19GEN4',
    'WEAPON_PMXFM',
    'WEAPON_MAC10',
    'WEAPON_MK47FM',
    'WEAPON_M6IC',
    'WEAPON_SCARSC',
    'WEAPON_M4',
    'WEAPON_AK47',
    'WEAPON_AK74',
    'WEAPON_AKS74',
    'WEAPON_GROZA',
    'WEAPON_SCARH',

```
## Drop the next code in ``qb-smallresources/client/recoil.lua (LINE 107)``

```lua
    [GetHashKey("weapon_flamethrower")] = 0.40,
	[GetHashKey("weapon_dragunov")] = 0.45,
	[GetHashKey("weapon_m24")] = 0.50,
	[GetHashKey("weapon_mpx")] = 0.60,
	[GetHashKey("weapon_m14")] = 0.55,
	[GetHashKey("weapon_skorpion")] = 0.30,
    [GetHashKey("weapon_g22")] = 0.40,
    [GetHashKey("weapon_ltl")] = 0.40,
    [GetHashKey("weapon_mp5")] = 0.50,
    [GetHashKey("weapon_dp9")] = 0.50,
	[GetHashKey("weapon_browning")] = 0.70,
    [GetHashKey("weapon_1911")] = 0.75,
    [GetHashKey("weapon_keyboard")] = 0.65,
    [GetHashKey("weapon_potatolauncher")] = 0.65,
	[GetHashKey("weapon_glock17")] = 0.40,
	[GetHashKey("weapon_glock18c")] = 0.45,
	[GetHashKey("weapon_glock22")] = 0.50,
	[GetHashKey("weapon_deagle")] = 0.60,
	[GetHashKey("weapon_fnx45")] = 0.55,
	[GetHashKey("weapon_m1911")] = 0.30,
    [GetHashKey("weapon_glock20")] = 0.40,
    [GetHashKey("weapon_glock19gen4")] = 0.40,
    [GetHashKey("weapon_pmxfm")] = 0.50,
    [GetHashKey("weapon_mac10")] = 0.50,
	[GetHashKey("weapon_mk47fm")] = 0.70,
    [GetHashKey("weapon_m6ic")] = 0.75,
    [GetHashKey("weapon_scarsc")] = 0.65,
    [GetHashKey("weapon_m4")] = 0.65,
    [GetHashKey("weapon_ak47")] = 0.65,
    [GetHashKey("weapon_ak74")] = 0.65,
    [GetHashKey("weapon_aks74")] = 0.75,
    [GetHashKey("weapon_groza")] = 0.75,
    [GetHashKey("weapon_scarh")] = 0.65,
```
## Add this next line of code to your weaponsTable in ``ps-dispatch/client/cl_events.lua``
```lua
    [GetHashKey("WEAPON_FLAMETHROWER")] = "CLASS 3: Flamethrower",
    [GetHashKey("WEAPON_DRAGUNOV")] = "CLASS 3: Dragunov",
    [GetHashKey("WEAPON_G22")] = "CLASS 4: G22 Sniper",
    [GetHashKey("WEAPON_LTL")] = "CLASS 2: Bean Bag Shotgun",
    [GetHashKey("WEAPON_MP5")] = "CLASS 2: MP5",
    [GetHashKey("WEAPON_DP9")] = "CLASS 1: DP9",
    [GetHashKey("WEAPON_BROWNING")] = "CLASS 1: Browning",
    [GetHashKey("WEAPON_1911")] = "CLASS 1: 1911",
    [GetHashKey("WEAPON_STAFF")] = "CLASS 99: GODS STAFF,
    [GetHashKey("WEAPON_GLOCK17")] = "CLASS 1: Glock-17",
    [GetHashKey("WEAPON_GLOCK18C")] = "CLASS 2: Glock-18 Custom",
    [GetHashKey("WEAPON_GLOCK22")] = "CLASS 1: Glock-22",
    [GetHashKey("WEAPON_DEAGLE")] = "CLASS 2: Desert Eagle",
    [GetHashKey("WEAPON_FNX45")] = "CLASS 1: FN FNX-45",
    [GetHashKey("WEAPON_M1911")] = "CLASS 1: M1911",
    [GetHashKey("WEAPON_GLOCK20")] = "CLASS 1: Glock-20",
    [GetHashKey("WEAPON_GLOCK19GEN4")] = "CLASS 1: Glock-19 Gen 4",
    [GetHashKey("WEAPON_PMXFM")] = "CLASS 2: Beretta PMX",
    [GetHashKey("WEAPON_MAC10")] = "CLASS 2: MAC-10",
    [GetHashKey("WEAPON_MK47FM")] = "CLASS 3: MK47 Mutant",
    [GetHashKey("WEAPON_M6IC")] = "CLASS 3: LWRC M6IC",
    [GetHashKey("WEAPON_SCARSC")] = "CLASS 3: Scar SC",
    [GetHashKey("WEAPON_M4")] = "CLASS 3: M4A1 Carbine",
    [GetHashKey("WEAPON_AK47")] = "CLASS 3: AK-47",
    [GetHashKey("WEAPON_AK74")] = "CLASS 3: AK-74",
    [GetHashKey("WEAPON_AKS74")] = "CLASS 3: AKS-74",
    [GetHashKey("WEAPON_GROZA")] = "CLASS 3: OTs-14 Groza",
    [GetHashKey("WEAPON_SCARH")] = "CLASS 3: Scar-H",
```
