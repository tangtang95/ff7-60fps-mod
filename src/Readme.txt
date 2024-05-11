FOR USERS
In order to fix few small FIELD mode animation glitches, double click on the mod to open configuration for the mods and enable
the fixes for 60FPS field mode. Remember that these small fixes are not compatible with other Gameplay or translation mods
(such as Echo-S and New Threat). Those mods needs to add these fixes on their own mod. 
So enable this only if you use original English FF7.


FOR MODDERS
Modifications to flevel.lgp FIELD maps:

 - blin70_2:
			in "Cloud - script 9", multiply by 2 the right value of the if (from 25 to 50)
                  in "Barret - script 11", multiply by 2 the right value of the if (from 30 to 60)
			 
			 
 - mds7st2:
			in "event - script 3":
			+change the order of execution kyak01/kisya02/kyak02 instead of kisya02/kyak02/kyak01.
			+set type of kyak2 in sync/wait option.
                  +set type of kyak01 in async/no wait option.

 
 - woa_2:
			in "woa2" in "S0-Init":
			+multiply by 2 all right values set to Var[5][17]
			
			in "woa2" in "Script 1":
			+multiply by 2 all right values set to Var[5][16]
			+multiply by 2 all right values set to Var[5][17]
			+multiply by 2 the values only in the LAST "Animate background layer #3"
 
 
 - woa_3: 
 			in "woa2" in "S0-Init":
			+multiply by 2 all right values set to Var[5][6]
			
			in "woa2" in "Script 1":
			+multiply by 2 all right values set to Var[5][5]
			+multiply by 2 all right values set to Var[5][6]
			+multiply by 2 the values only in the LAST "Animate background layer #3"
 - sinin2_1: This fixes the speed for the lock numbers
			in "cl" Script 3:
			+inside "if key[LEFT]" and "if key[RIGHT]" add "wait 1 frame" at the end and make it jump after "if key[OK]"
 - kuro_4: It fixes the clock synchronization and speed (thanks to @satsukiyatoshi)
                        in "mover" S0-Main: decrease +2 of Var[6][43] to +1
			  