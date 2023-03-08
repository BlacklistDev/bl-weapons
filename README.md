# bl-weapons

## Description ##

I am sorry i cannot put the download inside of my github, the file is to big. I will post a link below this to my google drive download, there you will have the files!
https://drive.google.com/drive/folders/1_4LxDoz3IPeOCVafqLNxx7C97ZLd8ANd?usp=share_link

## Setup ##

Please Follow These Steps

## Installation ##

-- Put the weapons file in your resources folder

## Drop this code in ``qb-core/shared/items.lua``
````
--Blacklist Custom WEAPONS
	['weapon_radargun'] 				 = {['name'] = 'weapon_radargun', 		      	['label'] = 'Radar Gun', 					['weight'] = 1000, 		['type'] = 'weapon', 	['ammotype'] = nil,						['image'] = 'weapon_radargun.png', 		['unique'] = true, 		['useable'] = false, 	['description'] = 'A handhel speed detection device'},
	['weapon_flamethrower'] 				 = {['name'] = 'weapon_flamethrower', 		['label'] = 'Flamethrower', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = nil,		['image'] = 'flamethrower.png', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_dragunov'] 				 = {['name'] = 'weapon_dragunov', 		['label'] = 'Dragunov', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = 'weapon_sniperrifle.png', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_mpx'] 						 = {['name'] = 'weapon_mpx', 	 	['label'] = 'MPX', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_m24'] 						 = {['name'] = 'weapon_m24', 	 	['label'] = 'M 24', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_m14'] 		 				 = {['name'] = 'weapon_m14', 	 	['label'] = 'MK14', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_g22'] 		 				 = {['name'] = 'weapon_g22', 	 	['label'] = 'PD G22 Sniper', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = 'weapon_heavysniper.png', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_skorpion'] 				 = {['name'] = 'weapon_skorpion', 	 	['label'] = 'Skorpion', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_ltl'] 		 				 = {['name'] = 'weapon_ltl', 	 	['label'] = 'PD Bean Bag Shotgun', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = 'weapon_pumpshotgun_mk2.png', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_mp5'] 		 				 = {['name'] = 'weapon_izh81', 	 	['label'] = 'MP 5', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = 'weapon_smg', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_dp9'] 		 				 = {['name'] = 'weapon_dp9', 	 	['label'] = 'PD DP9', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = 'weapon_dp9.png', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_browning'] 		 		 = {['name'] = 'weapon_browning', 	 		['label'] = 'Browning', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_1911'] 		 		  	 = {['name'] = 'weapon_1911', 	 			['label'] = 'M 1911', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_keyboard'] 		 	     = {['name'] = 'weapon_keyboard', 	 		['label'] = 'Keyboard', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_potatolauncher'] 		 	 = {['name'] = 'weapon_potatolauncher', 	['label'] = 'Potato Launcher', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = '', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_staff'] 		 			 = {['name'] = 'weapon_staff', 	 			['label'] = 'Staff', 		['weight'] = 1000, 		['type'] = 'weapon', 		['ammotype'] = 'AMMO_SNIPER',		['image'] = 'staff.png', 	 ['unique'] = true, 	['useable'] = false, 	['description'] = 'A high-precision, long-range rifle'},
	['weapon_katana'] 				 = {['name'] = 'weapon_katana', 	 		  	['label'] = 'Katana', 					['weight'] = 2000, 		['type'] = 'weapon', 	['ammotype'] = nil,						['image'] = 'weapon_katana.png', 			['unique'] = true, 		['useable'] = false,	['description'] = 'A single-edged sword that is the longer of a pair worn by the Japanese samurai.'},
    ['weapon_shiv'] 				 = {['name'] = 'weapon_shiv', 	 		  		['label'] = 'Shiv', 					['weight'] = 1000, 		['type'] = 'weapon', 	['ammotype'] = nil,						['image'] = 'weapon_shiv.png', 				['unique'] = true, 		['useable'] = false,	['description'] = 'An instrument composed of a blade fixed into a handle, used for cutting or as a weapon.'},
    ['weapon_sledgehammer'] 		 = {['name'] = 'weapon_sledgehammer', 	 		['label'] = 'Sledge Hammer', 			['weight'] = 9000, 		['type'] = 'weapon', 	['ammotype'] = nil,						['image'] = 'weapon_sledgehammer.png', 		['unique'] = true, 		['useable'] = false,	['description'] = 'A Sledge Hammer to destroy peoples heads... jk... unless...'},
    ['weapon_karambit'] 			 = {['name'] = 'weapon_karambit', 			 	['label'] = 'Karambit', 				['weight'] = 1000, 		['type'] = 'weapon', 	['ammotype'] = nil,						['image'] = 'weapon_karambit.png', 		    ['unique'] = true, 		['useable'] = false,	['description'] = 'A short knife with a pointed and edged blade, used as a weapon'},
	['weapon_glock17'] 				 = {['name'] = 'weapon_glock17', 				['label'] = 'Glock-17', 				['weight'] = 7000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_glock17.png', 			['unique'] = true, 		['useable'] = false,	['description'] = 'The Glock 17 is the original 9×19mm Parabellum model, with a standard magazine capacity of 17 rounds.'},
	['weapon_glock18c'] 			 = {['name'] = 'weapon_glock18c', 				['label'] = 'Glock-18C', 				['weight'] = 7000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_glock18c.png', 			['unique'] = true, 		['useable'] = false,	['description'] = 'The Glock 18C is a selective-fire variant of the Glock 17.'},
	['weapon_glock22'] 			     = {['name'] = 'weapon_glock22', 				['label'] = 'Glock-22', 				['weight'] = 7000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_glock22.png', 			['unique'] = true, 		['useable'] = false,	['description'] = 'The Glock 22 is a .40 S&W version of the full-sized Glock 17.'},
	['weapon_deagle'] 					 = {['name'] = 'weapon_deagle', 			['label'] = 'Desert Eagle',			    ['weight'] = 8000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_deagle.png', 			['unique'] = true, 		['useable'] = false,	['description'] = 'The Desert Eagle is a gas-operated, semi-automatic pistol known for chambering the .50 Action Express, the largest centerfire cartridge of any magazine-fed, self-loading pistol.'},
	['weapon_fnx45'] 				 = {['name'] = 'weapon_fnx45', 	 				['label'] = 'FN FNX-45', 				['weight'] = 7000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_fnx45.png', 			['unique'] = true, 		['useable'] = false,	['description'] = 'The FN FNX pistol is a series of semi-automatic, the pistol is chambered for the 9×19mm Parabellum, .40 S&W, and .45 ACP cartridges.'},
	['weapon_m1911'] 				 = {['name'] = 'weapon_m1911', 	 			  	['label'] = 'M1911', 					['weight'] = 7000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_m1911.png',  			['unique'] = true, 		['useable'] = false,	['description'] = 'The M1911 (Colt 1911 or Colt Government) is a single-action, recoil-operated, semi-automatic pistol chambered for the .45 ACP cartridge.'},
    ['weapon_glock20'] 				 = {['name'] = 'weapon_glock20', 	 			['label'] = 'Glock-20', 				['weight'] = 7000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_glock20.png',  			['unique'] = true, 		['useable'] = false,	['description'] = 'An ambidextrous, reversible magazine latch makes the GLOCK 20 an ideal handgun for right- and left-handed shooters.'},
    ['weapon_glock19gen4'] 			 = {['name'] = 'weapon_glock19gen4', 	 		['label'] = 'Glock-19 Gen 4', 			['weight'] = 7000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_glock19gen4.png',  		['unique'] = true, 		['useable'] = false,	['description'] = 'The GLOCK 19 Gen4 pistol in 9 mm Luger offers great firepower while allowing to shoot quick and accurately.'},
    ['weapon_pmxfm'] 				 = {['name'] = 'weapon_pmxfm', 	 			  	['label'] = 'Beretta PMX', 				['weight'] = 11000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_SMG',				['image'] = 'weapon_pmxfm.png',  			['unique'] = true, 		['useable'] = false,	['description'] = 'The Beretta PMX is a 9x19mm Parabellum caliber submachine gun, designed and manufactured by the Italian company Beretta.'},
    ['weapon_mac10'] 				 = {['name'] = 'weapon_mac10', 			 		['label'] = 'MAC-10', 					['weight'] = 10000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_SMG',				['image'] = 'weapon_mac10.png', 			['unique'] = true, 		['useable'] = false, 	['description'] = 'The Military Armament Corporation Model 10, commonly known as the MAC 10 and also known as the M10 or MAC-10.'},
    ['weapon_mk47fm'] 				 = {['name'] = 'weapon_mk47fm', 	 			['label'] = 'MK47 Mutant', 				['weight'] = 16000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_mk47fm.png',  			['unique'] = true, 		['useable'] = false,	['description'] = 'The Mk47 Mutant is an American-made semi-automatic rifle chambered in 7.62×39mm caliber.'},
    ['weapon_m6ic'] 				 = {['name'] = 'weapon_m6ic', 	 			  	['label'] = 'LWRC M6IC', 				['weight'] = 14000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_m6ic.png',  			['unique'] = true, 		['useable'] = false,	['description'] = 'The LWRC M6IC is an AR-15 direct impingement rifle made by LWRC and was created for the US Military.'},
    ['weapon_scarsc'] 				 = {['name'] = 'weapon_scarsc', 	 			['label'] = 'Scar SC', 					['weight'] = 14000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_scarsc.png',  			['unique'] = true, 		['useable'] = false,	['description'] = 'The FN SCAR-SC is offered in the U.S. as select-fire only with a non-reciprocating charging handle and telescoping buttstock.'},
    ['weapon_m4'] 					 = {['name'] = 'weapon_m4', 	 			  	['label'] = 'M4A1 Carbine', 			['weight'] = 13000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_m4.png',			 	['unique'] = true, 		['useable'] = false,	['description'] = 'The M4 carbine is a 5.56×45mm NATO, gas-operated, magazine-fed carbine developed in the United States during the 1980s.'},
    ['weapon_ak47'] 		 		 = {['name'] = 'weapon_ak47', 	 			  	['label'] = 'AK-47', 					['weight'] = 13000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_ak47.png', 				['unique'] = true, 		['useable'] = false,	['description'] = 'The AK-47, officially known as the Avtomat Kalashnikova, is a gas-operated assault rifle that is chambered for the 7.62×39mm cartridge.'},
    ['weapon_ak74'] 		 		 = {['name'] = 'weapon_ak74', 	 			  	['label'] = 'AK-74', 					['weight'] = 13000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_ak74.png', 				['unique'] = true, 		['useable'] = false,	['description'] = 'The AK-74 or Kalashnikov automatic rifle model 1974 is a 5.45mm assault rifle developed in the early 1970s in the Soviet Union.'},
    ['weapon_aks74'] 		 		 = {['name'] = 'weapon_aks74', 	 			  	['label'] = 'AKS-74', 					['weight'] = 13000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_aks74.png', 			['unique'] = true, 		['useable'] = false,	['description'] = 'The AKS-74U Short Assault Rifle is a shortened version of the AKS-74 Assault Rifle released in 1979.'},
    ['weapon_groza'] 				 = {['name'] = 'weapon_groza', 			 		['label'] = 'OTs-14 Groza', 			['weight'] = 15000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_groza.png', 			['unique'] = true, 		['useable'] = false, 	['description'] = 'The OTs-14 Groza is a Russian selective fire bullpup assault rifle chambered for the 7.62×39 round and the 9×39mm subsonic round.'},
    ['weapon_scarh'] 				 = {['name'] = 'weapon_scarh', 	 				['label'] = 'Scar-H', 					['weight'] = 14000, 	['type'] = 'weapon', 	['ammotype'] = 'AMMO_RIFLE',			['image'] = 'weapon_scarh.png',  			['unique'] = true, 		['useable'] = false,	['description'] = 'The FN SCAR-H PR are highly accurate semi-auto or selective fire precision rifles for designated marksmen or sniper teams.'},
    
```  
## Drop The Next code in qb-core/shared/weapons.lua ##

-- Blacklist Custom Weapons
	[`weapon_radargun`] 				 = {['name'] = 'weapon_radargun', 		['label'] = 'Radar Gun', 				['ammotype'] = nil,	['damagereason'] = 'Really???'},
	[`weapon_dragunov`] 		 = {['name'] = 'weapon_dragunov', 	 	['label'] = 'Dragunov', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_draco`] 		 = {['name'] = 'weapon_draco', 	 	['label'] = 'Draco', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
	[`weapon_gepard`] 		 = {['name'] = 'weapon_gepard', 	 	['label'] = 'Gepard', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_groza`] 		 = {['name'] = 'weapon_groza', 	 	['label'] = 'Groza', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_scar`] 		 = {['name'] = 'weapon_scar', 	 	['label'] = 'Scar', 				['ammotype'] = 'AMMO_RIFLE',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_mpx`] 		 = {['name'] = 'weapon_mpx', 	 	['label'] = 'MPX', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_m24`] 		 = {['name'] = 'weapon_m24', 	 	['label'] = 'M24', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_m14`] 		 = {['name'] = 'weapon_m14', 	 	['label'] = 'M14', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_g22`] 		 = {['name'] = 'weapon_g22', 	 	['label'] = 'G22 Sniper', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_skorpion`] 		 = {['name'] = 'weapon_skorpion', 	 	['label'] = 'Skorpion', 				['ammotype'] = 'AMMO_SNIPER',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
	[`weapon_ltl`] 		 = {['name'] = 'weapon_ltl', 	 	['label'] = 'PD Bean Bag Shotgun', 				['ammotype'] = 'AMMO_SHOTGUN',	['damagereason'] = 'Ended / Sniped / Shot down / Floored'},
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
  [`weapon_glock18c`] 		 	= {['name'] = 'weapon_glock18c', 			['label'] = 'Glock-18 Custom',		    ['weapontype'] = 'Pistol',			['ammotype'] = 'AMMO_PISTOL',			['damagereason'] = 'Pistoled / Blasted / Plugged / Bust a cap in'},
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
  [`weapon_m4`] 		 			= {['name'] = 'weapon_m4', 	 				['label'] = 'M4A1 Carbine', 			['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
  [`weapon_ak47`] 		 		= {['name'] = 'weapon_ak47', 	 			['label'] = 'AK-47', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
  [`weapon_ak74`] 		 		= {['name'] = 'weapon_ak74', 	 			['label'] = 'AK-74', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
  [`weapon_aks74`] 		 		= {['name'] = 'weapon_aks74', 	 			['label'] = 'AKS-74', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
  [`weapon_groza`] 		 		= {['name'] = 'weapon_groza', 	 			['label'] = 'OTs-14 Groza', 			['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},
  [`weapon_scarh`] 		 		= {['name'] = 'weapon_scarh', 	 			['label'] = 'Scar-H', 					['weapontype'] = 'Assault Rifle',	['ammotype'] = 'AMMO_RIFLE',			['damagereason'] = 'Ended / Rifled / Shot down / Floored'},

## Drop The Next Code in ``qb-weapons/config.lua``

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

## Drop the next code in ``qb-weapons/config.lua``
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

## Add the next code in ``qb-smallresources/client/weapondraw.lua``

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
    'WEAPON_RADARGUN',

## Drop the next code in ``qb-smallresources/client/recoil.lua (LINE 107)``


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
    
## Add this next line of code to your weaponsTable in ``ps-dispatch/client/cl_events.lua``
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
