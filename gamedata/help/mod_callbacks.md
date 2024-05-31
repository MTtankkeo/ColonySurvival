﻿CallbackType: `AfterModsLoaded`  
=======  
Method type: System.Action<System.Collections.Generic.List<ModLoader.ModDescription>>  
Called after parsing all modinfo files  
Registered callbacks: 1  
0.	'create_filetable' -> 'ServerManager.AfterModsLoadedCreateFiletable'   


CallbackType: `OnItemTypeRegistered`  
=======  
Method type: System.Action<ItemTypes.ItemType>  
Called once for each type that is being registered to ItemTypes  
Registered callbacks: 3  
0.	'BlockEntities.Implementations.Astrolabe+Callbacks.OnItemTypeRegistered' -> 'BlockEntities.Implementations.Astrolabe+Callbacks.OnItemTypeRegistered'   
1.	'pipliz.server.itemtypesserver' -> 'ItemTypesServer.OnRegisteredItemType'   
2.	'register_tools' -> 'ItemTypesServer+Callbacks.OnItemTypeRegistered'   


CallbackType: `OnUpdateStart`  
=======  
Method type: System.Action  
Called early on in unity's Update method  
Registered callbacks: 5  
0.	'startmainthreadonly' -> 'ThreadPhase+Callbacks.OnUpdateStart' index: -1000000  
1.	'pipliz.server.setsecondsthisframe' -> 'Pipliz.Time.SetThisFrame' index: -1000  
2.	'servertime.startframe' -> 'ServerTime+ServerCallbacks.OnUpdateStart' index: -1000  
3.	'mainthreadactions' -> 'ThreadManager+Callbacks.OnUpdateStart' index: -100  
4.	'monstertracker.applythreadresults' -> 'Monsters.MonsterTracker+Callbacks.OnUpdateStart'   


CallbackType: `OnUpdate`  
=======  
Method type: System.Action  
In the middle of unity's Update method.  
Registered callbacks: 18  
0.	'steammanager' -> 'SteamManager+Callbacks.OnUpdate' index: -1000  
1.	'networkwrapper.receivemessages' -> 'NetworkWrapper+Callbacks.OnUpdate' index: -999  
2.	'BlockEntities.Implementations.Grass+Callbacks.OnUpdate' -> 'BlockEntities.Implementations.Grass+Callbacks.OnUpdate'   
3.	'colonytrackerupdate' -> 'ColonyTracker+Callbacks.OnUpdate'   
4.	'dotrading' -> 'ColonyTrading.Update'   
5.	'monstertracker.update' -> 'Monsters.MonsterTracker+Callbacks.OnUpdate'   
6.	'effectstracker' -> 'EffectsTracker.OnUpdate'   
		 Parent @ 5 : 'monstertracker.update'  
		 Child @ 8 : 'npctracker.update'  
7.	'Networking.NetworkSteamDiscovery+PlayerCountCacher.OnUpdate' -> 'Networking.NetworkSteamDiscovery+PlayerCountCacher.OnUpdate'   
8.	'npctracker.update' -> 'NPC.NPCTracker+Callbacks.OnUpdate'   
9.	'ChunkQueue.Update' -> 'ChunkQueue+Callbacks.OnUpdate' index: 100  
10.	'pipliz.server.chunkupdater' -> 'ChunkUpdating.Update'   
		 Parent @ 9 : 'ChunkQueue.Update'  
11.	'pipliz.server.tickscounter' -> 'Chatting.Commands.TicksPerSecond.Update'   
12.	'pipliz.server.updatetimecycle' -> 'TimeCycle.Update'   
13.	'players.update' -> 'Players+Callbacks.OnUpdate'   
14.	'savemanager.onupdate' -> 'Saving.SaveManager+Callbacks.OnUpdate'   
15.	'update_transports' -> 'Transport.TransportManager+Callbacks.OnUpdate'   
16.	'update_water' -> 'BlockEntities.Implementations.Water.Tick'   
17.	'updateblockentities' -> 'BlockEntities.BlockEntityTracker+Callbacks.OnUpdate'   


CallbackType: `OnUpdateEnd`  
=======  
Method type: System.Action  
At the end of unity's Update method.  
Registered callbacks: 4  
0.	'pipliz.server.senddirtystockpiles' -> 'StockpileManager.SendDirtyStockpiles'   
1.	'mainthreadactions' -> 'ThreadManager+Callbacks.OnUpdateEnd' index: 100  
2.	'networkwrapper.finishframe' -> 'NetworkWrapper+Callbacks.OnUpdateEnd' index: 500  
3.	'endmainthreadonly' -> 'ThreadPhase+Callbacks.OnUpdateEnd' index: 1000000  


CallbackType: `OnLateUpdate`  
=======  
Method type: System.Action  
Called inside unity's LateUpdate method  
Registered callbacks: 1  
0.	'servertime.endframe' -> 'ServerTime+ServerCallbacks.OnLateUpdate' index: 1000  


CallbackType: `AfterItemTypesDefined`  
=======  
Method type: System.Action  
First callback after all item types should be defined, so you can resolve types etc here  
Registered callbacks: 45  
0.	'initialize_upgrademanager' -> 'Assets.ColonyPointUpgrades.UpgradesManager+CallbacksA.AfterItemTypesDefined' index: -1001  
1.	'create_servermanager_trackers' -> 'ServerManager.CreateBlockEntityCallbacks' index: -1000  
2.	'process_smart_moulding' -> 'BlockEntities.Implementations.MouldingPlacement.AfterItemTypesDefined'   
		 Child @ 4 : 'blockentitycallback.autoloaders'  
3.	'register_smart_placement' -> 'BlockEntities.SmartPlacement.AfterItemTypesDefined'   
		 Child @ 4 : 'blockentitycallback.autoloaders'  
4.	'blockentitycallback.autoloaders' -> 'ServerManager.AutoLoadBlockEntities'   
		 Parent @ 1 : 'create_servermanager_trackers'  
5.	'chunk_dedupe_initializer' -> 'Chunk+ChunkDataDeduplicator.Initialize'   
6.	'NPC.NPCNames.AfterItemTypesDefined' -> 'NPC.NPCNames.AfterItemTypesDefined'   
		 Child @ 21 : 'pipliz.server.endloadcolonies'  
7.	'pipliz.server.loadnpctypes' -> 'NPC.NPCType.LoadNPCTypes'   
8.	'areajobs.insertattributed' -> 'AreaJobTracker.RegisterAutoDefs'   
		 Parent @ 7 : 'pipliz.server.loadnpctypes'  
9.	'parse_starterpack_patches_afteritemtype' -> 'StarterPacks.Loader.ParsePacks'   
		 Child @ 10 : 'pipliz.server.recipeload'  
10.	'pipliz.server.recipeload' -> 'Recipes.RecipeStorage+Callbacks.AfterItemTypesDefined'   
		 Parent @ 1 : 'create_servermanager_trackers'  
11.	'pipliz.server.loadresearchables' -> 'ServerManager.LoadResearchables'   
		 Parent @ 7 : 'pipliz.server.loadnpctypes'  
		 Parent @ 1 : 'create_servermanager_trackers'  
		 Parent @ 10 : 'pipliz.server.recipeload'  
12.	'pipliz.server.endloadplayers' -> 'Players.EndInitializePlayerData'   
13.	'createareajobdefinitions' -> 'AreaJobTracker+AreaJobPatches.CreateAreaJobDefinitions'   
		 Parent @ 7 : 'pipliz.server.loadnpctypes'  
14.	'bookcase_registers' -> 'BlockEntities.Implementations.Bookcases+Callbacks.AfterItemTypesDefined'   
		 Parent @ 1 : 'create_servermanager_trackers'  
		 Child @ 16 : 'pipliz.blocknpcs.registerjobs'  
15.	'wisteriatree_register' -> 'BlockEntities.Implementations.WisteriaTreeRegistration.AfterItemTypesDefined'   
		 Parent @ 1 : 'create_servermanager_trackers'  
		 Child @ 16 : 'pipliz.blocknpcs.registerjobs'  
16.	'pipliz.blocknpcs.registerjobs' -> 'Jobs.BlockJobLoader.AfterDefiningNPCTypes'   
		 Parent @ 1 : 'create_servermanager_trackers'  
		 Parent @ 7 : 'pipliz.server.loadnpctypes'  
		 Parent @ 4 : 'blockentitycallback.autoloaders'  
17.	'creategrowabledefinitions' -> 'GrowableBlocks.GrowablePatchHandler.CreateGrowableDefinitions'   
		 Parent @ 1 : 'create_servermanager_trackers'  
18.	'parse_elevatortypes' -> 'Transport.Elevator.ElevatorManager.AfterItemTypesDefined'   
		 Child @ 23 : 'pipliz.server.completeloadmiscworld'  
19.	'parse_railtypes' -> 'Transport.Rail.RailManager.AfterItemTypesDefined'   
		 Child @ 23 : 'pipliz.server.completeloadmiscworld'  
20.	'register_upgrades' -> 'Assets.ColonyPointUpgrades.UpgradesManager+CallbacksB.AfterItemTypesDefined' index: 10  
		 Parent @ 0 : 'initialize_upgrademanager'  
		 Parent @ 11 : 'pipliz.server.loadresearchables'  
		 Child @ 21 : 'pipliz.server.endloadcolonies'  
21.	'pipliz.server.endloadcolonies' -> 'ServerManager.LoadColonies'   
		 Parent @ 7 : 'pipliz.server.loadnpctypes'  
		 Parent @ 8 : 'areajobs.insertattributed'  
		 Parent @ 1 : 'create_servermanager_trackers'  
		 Parent @ 10 : 'pipliz.server.recipeload'  
		 Parent @ 11 : 'pipliz.server.loadresearchables'  
		 Parent @ 12 : 'pipliz.server.endloadplayers'  
		 Parent @ 13 : 'createareajobdefinitions'  
22.	'load_notifications' -> 'Notifications.NotificationCallbacks.AfterItemTypesDefined'   
		 Parent @ 21 : 'pipliz.server.endloadcolonies'  
		 Child @ 23 : 'pipliz.server.completeloadmiscworld'  
23.	'pipliz.server.completeloadmiscworld' -> 'ServerManager.CompleteLoadMiscWorld'   
		 Parent @ 21 : 'pipliz.server.endloadcolonies'  
		 Child @ 24 : 'start_load_startup_chunks'  
24.	'start_load_startup_chunks' -> 'ServerManager.CreateBlockEntityTracker' index: -1000  
		 Parent @ 4 : 'blockentitycallback.autoloaders'  
		 Parent @ 5 : 'chunk_dedupe_initializer'  
		 Parent @ 21 : 'pipliz.server.endloadcolonies'  
		 Parent @ 16 : 'pipliz.blocknpcs.registerjobs'  
		 Parent @ 17 : 'creategrowabledefinitions'  
25.	'BlockEntities.Implementations.Grass+Callbacks.AfterItemTypesDefined' -> 'BlockEntities.Implementations.Grass+Callbacks.AfterItemTypesDefined'   
26.	'BlockEntities.Implementations.PlayerSaplings+Callbacks.AfterItemTypesDefined' -> 'BlockEntities.Implementations.PlayerSaplings+Callbacks.AfterItemTypesDefined'   
27.	'monstertracker.load' -> 'Monsters.MonsterTracker+Callbacks.AfterItemTypesDefined'   
		 Parent @ 21 : 'pipliz.server.endloadcolonies'  
28.	'effectstracker_load' -> 'EffectsTracker.AfterItemTypesDefined'   
		 Parent @ 1 : 'create_servermanager_trackers'  
		 Parent @ 27 : 'monstertracker.load'  
29.	'find_auto_chatcommands' -> 'Chatting.CommandManager.Initialize'   
30.	'GrowableBlocks.SaplingHandler.AfterItemTypesDefined' -> 'GrowableBlocks.SaplingHandler.AfterItemTypesDefined'   
31.	'Jobs.ToolSetManager.AfterItemTypesDefined' -> 'Jobs.ToolSetManager.AfterItemTypesDefined'   
32.	'pipliz.server.asyncloadpermissions' -> 'PermissionsManager.Reload'   
33.	'pipliz.server.endblackandwhitelisting' -> 'BlackAndWhitelisting.EndReload'   
34.	'pipliz.server.endloadwater' -> 'BlockEntities.Implementations.Water.Load'   
35.	'pipliz.server.loadnpcmeshes' -> 'NPC.NPCType.LoadNPCMeshes'   
36.	'process_paintables' -> 'BlockEntities.Implementations.Paint.Paintables.AfterItemTypesDefined'   
37.	'process_smart_flowerbox' -> 'BlockEntities.Implementations.FlowerboxPlacement.AfterItemTypesDefined'   
38.	'process_smart_lantern' -> 'BlockEntities.Implementations.LanternPlacement.AfterItemTypesDefined'   
39.	'process_smart_rail_placement' -> 'BlockEntities.Implementations.SmartRailPlacement.AfterItemTypesDefined'   
40.	'process_smart_signs' -> 'BlockEntities.Implementations.SignPlacement.AfterItemTypesDefined'   
41.	'trading.doublelinkrules' -> 'ColonyTrading.LoadColonies'   
		 Parent @ 21 : 'pipliz.server.endloadcolonies'  
42.	'wait_complete_startup_chunks' -> 'ServerManager.WaitForCompletedStartupChunks' index: 1000  
		 Parent @ 24 : 'start_load_startup_chunks'  
43.	'set_colony_sciencemask' -> 'Science.ScienceManager+Callbacks.AfterItemTypesDefined' index: 1  
		 Parent @ 42 : 'wait_complete_startup_chunks'  
		 Parent @ 21 : 'pipliz.server.endloadcolonies'  
		 Parent @ 1 : 'create_servermanager_trackers'  
44.	'prepare_network_packets' -> 'ItemTypesServer+Callbacks.AfterItemTypesDefined' index: 10000  


CallbackType: `OnQuit`  
=======  
Method type: System.Action  
Called in the quit method queue  
Registered callbacks: 12  
0.	'pipliz.shared.waitforasyncquitsearly' -> 'Pipliz.Application.WaitForQuits' index: -1000  
1.	'BlockEntities.BlockEntityCallbacks+Callbacks.OnQuit' -> 'BlockEntities.BlockEntityCallbacks+Callbacks.OnQuit'   
2.	'close_filetable' -> 'FileTable+Callbacks.OnQuit'   
3.	'EffectsTracker.OnQuit' -> 'EffectsTracker.OnQuit'   
4.	'Monsters.MonsterSpawner+Callbacks.OnQuit' -> 'Monsters.MonsterSpawner+Callbacks.OnQuit'   
5.	'TerrainGeneration2.TerrainGenerator2ModManager.OnQuit' -> 'TerrainGeneration2.TerrainGenerator2ModManager.OnQuit'   
6.	'trigger_autosave' -> 'Saving.SaveManager+Callbacks2.OnQuit'   
7.	'steamnetworking.close' -> 'Pipliz.Networking.SteamNetworking+ModRegistering.OnQuit' index: 1  
8.	'pipliz.jointhreads' -> 'Pipliz.Threading.ThreadSafeQuitWrapper.JoinThread' index: 500  
9.	'close_savemanager' -> 'Saving.SaveManager+Callbacks.OnQuit' index: 750  
10.	'pipliz.shared.waitforasyncquitslate' -> 'Pipliz.Application.WaitForQuits' index: 1000  
11.	'LZ4DecoderFreeing' -> 'Pipliz.LZ4.LZ4Codec+Callbacks.OnQuit' index: 10000  


CallbackType: `AfterSelectedWorld`  
=======  
Method type: System.Action  
First callback after the world to load has been determined  
Registered callbacks: 12  
0.	'pipliz.server.loadaudiofiles' -> 'AudioManager.LoadAudioFiles' index: -100  
1.	'pipliz.server.applytexturemappingpatches' -> 'ItemTypesServer.ApplyTextureMappingPatches'   
2.	'pipliz.server.registertexturemappingtextures' -> 'ItemTypesServer.RegisterTextures' index: -100  
		 Parent @ 1 : 'pipliz.server.applytexturemappingpatches'  
3.	'registernpctextures' -> 'ItemTypesServer.RegisterNPCTextures' index: -100  
4.	'start_load_vehicle_meshes' -> 'Transport.TransportManager+Callbacks.AfterSelectedWorld' index: -100  
5.	'allocate_chunkqueue' -> 'ChunkQueue+Callbacks.AfterSelectedWorld'   
6.	'create_savemanager' -> 'ServerManager.CreateSaveManager'   
7.	'load_npc_mapping' -> 'NPC.NPCTypeID+Callbacks.AfterSelectedWorld'   
8.	'load_worldsettings' -> 'ServerManager.LoadWorldSettings'   
		 Parent @ 6 : 'create_savemanager'  
9.	'pipliz.imagemanager.loadingimages' -> 'Pipliz.ImageManager.AfterWorldLoad'   
10.	'pipliz.server.loadtimecycle' -> 'TimeCycle.Initialize'   
		 Parent @ 8 : 'load_worldsettings'  
11.	'pipliz.server.startblackandwhitelisting' -> 'BlackAndWhitelisting.StartReload'   


CallbackType: `AfterAddingBaseTypes`  
=======  
Method type: System.Action<System.Collections.Generic.Dictionary<string, ItemTypesServer.ItemTypeRaw>>  
Callback after AddItemTypes but before parsing those types; intended usecase is to allow changing the raw json  
No registered uses  


CallbackType: `AfterWorldLoad`  
=======  
Method type: System.Action  
Most things should be initialized by now, does not have to include chunks and pathing data though (those may be ongoing on other threads)  
Registered callbacks: 2  
0.	'pipliz.server.localization.convert' -> 'Localization.Convert'   
1.	'pipliz.server.monsterspawner.register' -> 'Monsters.MonsterSpawner+Callbacks.AfterWorldLoad'   


CallbackType: `AfterNetworkSetup`  
=======  
Method type: System.Action  
After the networkwrapper clas is ready to send data. Can take a few seconds for steam servers to connect.  
No registered uses  


CallbackType: `OnFixedUpdate`  
=======  
Method type: System.Action  
Unity's OnFixedUpdate method. See unity documentation.  
Registered callbacks: 1  
0.	'collisionchecker' -> 'Transport.CollisionChecker.FixedUpdate'   


CallbackType: `OnApplicationFocus`  
=======  
Method type: System.Action<bool>  
Unity's OnApplicationFocus method. See unity documentation.  
No registered uses  


CallbackType: `OnApplicationPause`  
=======  
Method type: System.Action<bool>  
Unity's OnApplicationPause method. See unity documentation.  
No registered uses  


CallbackType: `OnPlayerConnectedEarly`  
=======  
Method type: System.Action<Players.Player>  
Early on in the player connection process - the player is probably not ready to receive messages yet  
Registered callbacks: 2  
0.	'pipliz.server.sendinitialtime' -> 'TimeCycle.SendHeartBeat'   
1.	'pipliz.server.start_loadsurroundings' -> 'ChunkQueue+Callbacks.OnPlayerConnectedEarly'   


CallbackType: `OnPlayerDisconnected`  
=======  
Method type: System.Action<Players.Player>  
Registered callbacks: 4  
0.	'BlockEntities.Implementations.Astrolabe+Callbacks.OnPlayerDisconnected' -> 'BlockEntities.Implementations.Astrolabe+Callbacks.OnPlayerDisconnected'   
1.	'BlockEntities.Implementations.Sign.SignTracker+SignSender.OnPlayerDisconnected' -> 'BlockEntities.Implementations.Sign.SignTracker+SignSender.OnPlayerDisconnected'   
2.	'Jobs.CommandToolManager+ConstructionMenuHelper.OnPlayerDisconnected' -> 'Jobs.CommandToolManager+ConstructionMenuHelper.OnPlayerDisconnected'   
3.	'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnPlayerDisconnected' -> 'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnPlayerDisconnected'   


CallbackType: `OnSavingPlayer`  
=======  
Method type: System.Action<Newtonsoft.Json.Linq.JObject, Players.Player>  
Allows saving custom data into the player save file  
No registered uses  


CallbackType: `OnLoadingPlayer`  
=======  
Method type: System.Action<Newtonsoft.Json.Linq.JObject, Players.Player>  
Allows loading custom data saved with OnSavingPlayer  
No registered uses  


CallbackType: `OnSavedChunk`  
=======  
Method type: System.Action<Chunk>  
No registered uses  


CallbackType: `OnLoadedChunk`  
=======  
Method type: System.Action<Chunk>  
No registered uses  


CallbackType: `OnPlayerMoved`  
=======  
Method type: System.Action<Players.Player, UnityEngine.Vector3>  
Probably called about 6/second/player. New data is on the player already.  
Registered callbacks: 2  
0.	'BlockEntities.Implementations.Sign.SignTracker+SignSender.OnPlayerMoved' -> 'BlockEntities.Implementations.Sign.SignTracker+SignSender.OnPlayerMoved'   
1.	'pipliz.server.loadsurroundings' -> 'ChunkQueue+Callbacks.OnPlayerMoved'   


CallbackType: `OnModifyResearchables`  
=======  
Method type: System.Action<System.Collections.Generic.Dictionary<string, Science.IResearchable>>  
Called inside of OnAddResearchables - allows modifying researches added through jsonFiles before they're registered  
Registered callbacks: 1  
0.	'Recipes.RecipeStorage+Callbacks.OnModifyResearchables' -> 'Recipes.RecipeStorage+Callbacks.OnModifyResearchables'   


CallbackType: `OnChangedBlock`  
=======  
Method type: System.Action<ModLoader.OnTryChangeBlockData>  
Called after OnTryChangeBlock, if the block was actually succesfully changed.  
Registered callbacks: 1  
0.	'update_collisions' -> 'Transport.CollisionChecker.UpdateCollisions'   


CallbackType: `OnTryChangeBlock`  
=======  
Method type: System.Action<ModLoader.OnTryChangeBlockData>  
Callback triggered upon a call to ServerManager.TryChangeBlock - used by various code and the client to edit blocks  
Nothing changed yet when this callback happens and the change can be blocked.  
You can block is by setting CallbackState to Cancelled  
Registered callbacks: 2  
0.	'GrowableBlocks.SaplingHandler.OnTryChangeBlock' -> 'GrowableBlocks.SaplingHandler.OnTryChangeBlock'   
1.	'preventaccidentalbannerremoval' -> 'ServerManager.TempBannerFix'   


CallbackType: `OnPlayerConnectedLate`  
=======  
Method type: System.Action<Players.Player>  
Messages send here will work unlike with OnPlayerConnectedEarly. May be delayed till after the client is done loading.  
Registered callbacks: 6  
0.	'pipliz.imagemanager.sendimagesettings' -> 'Pipliz.ImageManager.OnPlayerConnectedEarly' index: -1000  
1.	'BlockEntities.Implementations.Sign.SignTracker+SignSender.OnPlayerConnectedLate' -> 'BlockEntities.Implementations.Sign.SignTracker+SignSender.OnPlayerConnectedLate'   
2.	'pipliz.server.meshedobjects.sendtable' -> 'MeshedObjects.MeshedObjectType.OnPlayerConnectedLate'   
3.	'pipliz.server.sendcheatstate' -> 'Chatting.Commands.DisableAchievements+Callbacks.OnPlayerConnectedLate'   
4.	'pipliz.server.sendnpctypes' -> 'NPC.NPCType.SendNPCTypes'   
5.	'send_attached_mesh' -> 'MeshedObjects.MeshedObjectManager.SendAttachedMesh'   
		 Parent @ 2 : 'pipliz.server.meshedobjects.sendtable'  


CallbackType: `OnAddResearchables`  
=======  
Method type: System.Action  
The place to add researchables to Server.Science.ScienceManager  
Registered callbacks: 1  
0.	'registerresearchables' -> 'Science.ScienceManager+Callbacks.OnAddResearchables'   


CallbackType: `OnConstructTooltipUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.ConstructTooltipUIData>  
Registered callbacks: 3  
0.	'button_startcolony' -> 'NetworkUI.NetworkMenuManager+BannerPlacementCallbacks.OnConstructTooltipUI'   
1.	'Jobs.CommandToolManager.OnConstructTooltipUI' -> 'Jobs.CommandToolManager.OnConstructTooltipUI'   
2.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager.ConstructTooltip'   


CallbackType: `OnNPCCraftedRecipe`  
=======  
Method type: System.Action<Jobs.IJob, Recipes.Recipe, System.Collections.Generic.List<Recipes.RecipeResult>>  
The results list is re-used, don't store it.  
Results can be edited. After the callback they'll be added to the npc/block's inventory  
If the results are not empty, the npc will show a npc indicator with a weighted random type from the non-optional results  
Registered callbacks: 2  
0.	'resolve.chances' -> 'Jobs.CallbackImplementations+GatherItemResolver.OnNPCCraftedRecipe' index: 10  
1.	'registerproduction' -> 'Jobs.CallbackImplementations+RegisterProductionStats.OnNPCCraftedRecipe'   
		 Parent @ 0 : 'resolve.chances'  


CallbackType: `OnPlayerDeath`  
=======  
Method type: System.Action<Players.Player>  
Registered callbacks: 1  
0.	'pipliz.server.onplayerdeath' -> 'Players.OnDeath'   


CallbackType: `OnPlayerRespawn`  
=======  
Method type: System.Action<Players.Player>  
Registered callbacks: 1  
0.	'pipliz.server.onplayerrespawn' -> 'Players.OnDeathReset'   


CallbackType: `OnMonsterSpawned`  
=======  
Method type: System.Action<Monsters.IMonster>  
No registered uses  


CallbackType: `OnMonsterHit`  
=======  
Method type: System.Action<Monsters.IMonster, ModLoader.OnHitData>  
No registered uses  


CallbackType: `OnMonsterDied`  
=======  
Method type: System.Action<Monsters.IMonster>  
No registered uses  


CallbackType: `OnNPCRecruited`  
=======  
Method type: System.Action<NPC.NPCBase>  
Registered callbacks: 1  
0.	'pipliz.server.jobfinderdirty' -> 'Jobs.JobFinder+Callbacks.OnNPCRecruited'   


CallbackType: `OnNPCDied`  
=======  
Method type: System.Action<NPC.NPCBase>  
Registered callbacks: 1  
0.	'pipliz.server.jobfinderdirty' -> 'Jobs.JobFinder+Callbacks.OnNPCDied'   


CallbackType: `OnNPCJobChanged`  
=======  
Method type: System.Action<System.ValueTuple<NPC.NPCBase, Jobs.IJob, Jobs.IJob>>  
Registered callbacks: 1  
0.	'pipliz.server.refundrecruitement' -> 'Jobs.JobFinder+Callbacks.OnNPCJobChanged'   


CallbackType: `OnNPCHit`  
=======  
Method type: System.Action<NPC.NPCBase, ModLoader.OnHitData>  
Registered callbacks: 1  
0.	'NPC.NPCBase+Callbacks.OnNPCHit' -> 'NPC.NPCBase+Callbacks.OnNPCHit'   


CallbackType: `OnPlayerClicked`  
=======  
Method type: System.Action<Players.Player, Shared.PlayerClickedData>  
Registered callbacks: 17  
0.	'BlockEntities.Implementations.AlarmbellTracker+Callbacks.OnPlayerClicked' -> 'BlockEntities.Implementations.AlarmbellTracker+Callbacks.OnPlayerClicked'   
1.	'BlockEntities.Implementations.Door.DoorTracker+Callbacks.OnPlayerClicked' -> 'BlockEntities.Implementations.Door.DoorTracker+Callbacks.OnPlayerClicked'   
2.	'BlockEntities.Implementations.Failsafes+Callbacks.OnPlayerClicked' -> 'BlockEntities.Implementations.Failsafes+Callbacks.OnPlayerClicked'   
3.	'BlockEntities.Implementations.Sign.SignTracker+Callbacks.OnPlayerClicked' -> 'BlockEntities.Implementations.Sign.SignTracker+Callbacks.OnPlayerClicked'   
4.	'check_banner_click' -> 'NetworkUI.NetworkMenuManager.CheckBannerClick'   
5.	'clicked_glider' -> 'Transport.Glider+Callbacks.OnPlayerClicked'   
		 Child @ 6 : 'clicked_transport'  
6.	'clicked_transport' -> 'Transport.TransportManager+Callbacks.OnPlayerClicked'   
7.	'Jobs.CommandToolManager.OnPlayerClicked' -> 'Jobs.CommandToolManager.OnPlayerClicked'   
8.	'pipliz.server.players.hitnpc' -> 'NetworkUI.NetworkMenuManager+CallbackConsumers.OnPlayerClicked'   
9.	'Transport.Elevator.ElevatorManager.OnPlayerClicked' -> 'Transport.Elevator.ElevatorManager.OnPlayerClicked'   
10.	'Transport.Rail.RailManager.OnPlayerClicked' -> 'Transport.Rail.RailManager.OnPlayerClicked'   
11.	'use_paint' -> 'BlockEntities.Implementations.Paint.Paintables.OnPlayerClicked'   
12.	'use_smart_flowerbox' -> 'BlockEntities.Implementations.FlowerboxPlacement.OnPlayerClicked'   
13.	'use_smart_lantern' -> 'BlockEntities.Implementations.LanternPlacement.OnPlayerClicked'   
14.	'use_smart_moulding' -> 'BlockEntities.Implementations.MouldingPlacement.OnPlayerClicked'   
15.	'use_smart_rail_placement' -> 'BlockEntities.Implementations.SmartRailPlacement.OnPlayerClicked'   
16.	'use_smart_sign' -> 'BlockEntities.Implementations.SignPlacement.OnPlayerClicked'   


CallbackType: `OnPlayerHit`  
=======  
Method type: System.Action<Players.Player, ModLoader.OnHitData>  
No registered uses  


CallbackType: `OnAutoSaveWorld`  
=======  
Method type: System.Action  
Triggers an autosave every x minutes, to begin autosaving non-block data (jobs, npc's, players)  
Registered callbacks: 14  
0.	'start_world_transaction' -> 'Saving.SaveManager+Callbacks2.OnAutoSaveWorld' index: -100  
1.	'BlockEntities.Implementations.Grass+Callbacks.OnAutoSaveWorld' -> 'BlockEntities.Implementations.Grass+Callbacks.OnAutoSaveWorld'   
2.	'effectstracker' -> 'EffectsTracker.OnAutoSaveWorld'   
3.	'pipliz.server.autosaveplayers' -> 'Players.SavePlayers'   
4.	'pipliz.server.autosavewater' -> 'BlockEntities.Implementations.Water.Save'   
5.	'pipliz.server.saveareajobs' -> 'ServerManager.SaveAreaJobs'   
6.	'pipliz.server.savecolonies' -> 'ServerManager.SaveColonies'   
7.	'pipliz.server.savemiscworld' -> 'ServerManager.SaveMiscWorld'   
8.	'pipliz.server.savemonsters' -> 'ServerManager.SaveMonsters'   
9.	'pipliz.server.savenpcs' -> 'ServerManager.SaveNPCs'   
10.	'pipliz.server.saveworldsettings' -> 'ServerManager.SaveWorldSettings'   
11.	'save_dirty_notifications' -> 'Notifications.NotificationCallbacks.OnAutoSaveWorld'   
12.	'save_jobconfig' -> 'JobConfigManager+Callbacks.OnAutoSaveWorld'   
13.	'end_world_transaction' -> 'Saving.SaveManager+Callbacks.OnAutoSaveWorld' index: 100  


CallbackType: `OnNPCGathered`  
=======  
Method type: System.Action<Jobs.IJob, Pipliz.Vector3Int, System.Collections.Generic.List<ItemTypes.ItemTypeDrops>>  
Can edit the results; don't store them - the list is re-used.  
After the callback, results will be added to the npc's inventory.  
The location does not have to be the job/npc's position - see the construction jobs.  
Registered callbacks: 2  
0.	'resolve.chances' -> 'Jobs.CallbackImplementations+GatherItemResolver.OnNPCGathered' index: 10  
1.	'registerproduction' -> 'Jobs.CallbackImplementations+RegisterProductionStats.OnNPCGathered'   
		 Parent @ 0 : 'resolve.chances'  


CallbackType: `OnShouldKeepChunkLoaded`  
=======  
Method type: System.Action<ChunkUpdating.KeepChunkLoadedData>  
!!! Will be called from multiple threads, simultaneously !!!  
Periodically triggered for every chunk loaded. Use it to keep chunks loaded - and to indicate how long you expect them to stay loaded.  
{data.CheckedChunk} -> the chunk  
{data.MillisecondsTillNextCheck} -> the minimum time until another callback will be fired. Defaults to random between 24000 and 64000  
{data.Result} -> bool indicating whether or not to keep this chunk. Defaults to false (set to true to keep it)  
{data.ChunkLoadedSource} -> source for this callback. If loadedstorage / loadedgenerator, the chunk is already locked for writing. if Updater, it is not locked.  
Registered callbacks: 4  
0.	'bannercheck' -> 'BlockEntities.Implementations.BannerTracker.CheckKeepChunkLoaded'   
1.	'pipliz.server.playercheck' -> 'Players.ShouldKeepChunkAlive'   
		 Parent @ 0 : 'bannercheck'  
2.	'check_blockentities' -> 'ServerManager.KeepBlockEntitiesLoaded'   
		 Parent @ 1 : 'pipliz.server.playercheck'  
3.	'constructionarea.check' -> 'Jobs.Implementations.Construction.ConstructionManager+Callbacks.OnShouldKeepChunkLoaded' index: 1000  


CallbackType: `AddItemTypes`  
=======  
Method type: System.Action<System.Collections.Generic.Dictionary<string, ItemTypesServer.ItemTypeRaw>>  
Registered callbacks: 3  
0.	'blockgenerator.generateblocks' -> 'ItemTypesServer+BlockRotator.AddLitTypes'   
1.	'parse_starterpack_patches_additemtypes' -> 'StarterPacks.Loader.CreateTypes'   
2.	'pipliz.server.applymoditempatches' -> 'ItemTypesServer.ApplyPatches'   
		 Parent @ 1 : 'parse_starterpack_patches_additemtypes'  
		 Parent @ 0 : 'blockgenerator.generateblocks'  


CallbackType: `OnPlayerChangedNetworkUIStorage`  
=======  
Method type: System.Action<System.ValueTuple<Players.Player, Newtonsoft.Json.Linq.JObject, string>>  
Called when a player closes a networkmenu while some of its state was changed  
Registered callbacks: 1  
0.	'pipliz.parsenetui' -> 'NetworkUI.NetworkMenuManager.ReceiveWorldSettings'   


CallbackType: `OnPlayerPushedNetworkUIButton`  
=======  
Method type: System.Action<NetworkUI.ButtonPressCallbackData>  
Registered callbacks: 10  
0.	'Assets.UIGeneration.ColonyManageJobs.OnPlayerPushedNetworkUIButton' -> 'Assets.UIGeneration.ColonyManageJobs.OnPlayerPushedNetworkUIButton'   
1.	'Assets.UIGeneration.PointsUpgrades.OnPlayerPushedNetworkUIButton' -> 'Assets.UIGeneration.PointsUpgrades.OnPlayerPushedNetworkUIButton'   
2.	'BlockEntities.Implementations.Failsafes+Callbacks.OnPlayerPushedNetworkUIButton' -> 'BlockEntities.Implementations.Failsafes+Callbacks.OnPlayerPushedNetworkUIButton'   
3.	'BlockEntities.Implementations.Sign.SignTracker+Callbacks.OnPlayerPushedNetworkUIButton' -> 'BlockEntities.Implementations.Sign.SignTracker+Callbacks.OnPlayerPushedNetworkUIButton'   
4.	'button_opencolonytab' -> 'NetworkUI.NetworkMenuManager+BannerPlacementCallbacks.OnPlayerPushedNetworkUIButton'   
5.	'handle_colony_management' -> 'NetworkUI.NetworkMenuManager.HandleButtons'   
6.	'Jobs.CommandToolManager.OnPlayerPushedNetworkUIButton' -> 'Jobs.CommandToolManager.OnPlayerPushedNetworkUIButton'   
7.	'Jobs.CommandToolManager+ConstructionMenuHelper.OnPlayerPushedNetworkUIButton' -> 'Jobs.CommandToolManager+ConstructionMenuHelper.OnPlayerPushedNetworkUIButton'   
8.	'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnPlayerPushedNetworkUIButton' -> 'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnPlayerPushedNetworkUIButton'   
9.	'NetworkUI.NetworkMenuManager+ToolshopCallbacks.OnPlayerPushedNetworkUIButton' -> 'NetworkUI.NetworkMenuManager+ToolshopCallbacks.OnPlayerPushedNetworkUIButton'   


CallbackType: `OnSendAreaHighlights`  
=======  
Method type: System.Action<Players.Player, System.Collections.Generic.List<AreaJobTracker.AreaHighlight>, System.Collections.Generic.List<ushort>>  
Edit the highlights list, adding desired area highlights to be sent to the player.  
Edit the showWhileHoldingTypes to add/remove types that will show <all> areas when selected in the inventory  
You can manually trigger this callback through AreaJobTracker.SendData(player)  
Registered callbacks: 2  
0.	'pipliz.defaultholdingtypes' -> 'AreaJobTracker.GatherShowWhileHoldingTypes'   
1.	'pipliz.sendjobareas' -> 'AreaJobTracker.GatherJobHighlights'   


CallbackType: `OnActiveColonyChanges`  
=======  
Method type: System.Action<Players.Player, Colony, Colony>  
Registered callbacks: 5  
0.	'onchange' -> 'ServerManager.OnColonyChange' index: -1000  
1.	'resend_areajobs' -> 'AreaJobTracker.OnActiveColonyChange'   
2.	'sendconstructiondata' -> 'Jobs.Implementations.Construction.ConstructionManager.SendData'   
3.	'sendresearch' -> 'Science.ScienceManager+Callbacks.OnActiveColonyChanges'   
4.	'sendthreat' -> 'Difficulty.ColonyThreatLevel+Callbacks.OnActiveColonyChanges'   


CallbackType: `OnSavingColony`  
=======  
Method type: System.Action<Colony, Newtonsoft.Json.Linq.JObject>  
Registered callbacks: 2  
0.	'savebuiltin' -> 'ColonyTracker+Callbacks.OnSavingColony'   
1.	'savejobfinder' -> 'Jobs.JobFinder+Callbacks.OnSavingColony'   


CallbackType: `OnLoadingColony`  
=======  
Method type: System.Action<Colony, Newtonsoft.Json.Linq.JObject>  
Registered callbacks: 2  
0.	'loadbuiltin' -> 'ColonyTracker+Callbacks.OnLoadingColony'   
1.	'loadjobfinder' -> 'Jobs.JobFinder+Callbacks.OnLoadingColony'   


CallbackType: `OnSavingColonyGroup`  
=======  
Method type: System.Action<ColonyGroup, Newtonsoft.Json.Linq.JObject>  
Registered callbacks: 4  
0.	'save_cheatstate' -> 'ColonyGroup+CheatCallbacks.OnSavingColonyGroup'   
1.	'save_trade' -> 'ColonyTrading+Callbacks.OnSavingColonyGroup'   
2.	'save_upgradestate' -> 'Assets.ColonyPointUpgrades.ColonyUpgradeState+Callbacks.OnSavingColonyGroup'   
3.	'savebuiltin' -> 'ColonyTracker+Callbacks.OnSavingColonyGroup'   


CallbackType: `OnLoadingColonyGroup`  
=======  
Method type: System.Action<ColonyGroup, Newtonsoft.Json.Linq.JObject>  
Registered callbacks: 4  
0.	'load_cheatstate' -> 'ColonyGroup+CheatCallbacks.OnLoadingColonyGroup'   
1.	'load_trade' -> 'ColonyTrading+Callbacks.OnLoadingColonyGroup'   
2.	'load_upgradestate' -> 'Assets.ColonyPointUpgrades.ColonyUpgradeState+Callbacks.OnLoadingColonyGroup'   
3.	'loadbuiltin' -> 'ColonyTracker+Callbacks.OnLoadingColonyGroup'   


CallbackType: `OnPlayerEditedNetworkInputfield`  
=======  
Method type: System.Action<NetworkUI.InputfieldEditCallbackData>  
Registered callbacks: 1  
0.	'handle_builtin' -> 'NetworkUI.NetworkMenuManager.HandleInputfields'   


CallbackType: `OnCreatedColony`  
=======  
Method type: System.Action<Colony>  
Called when a colony is created, does not trigger on loading colonies (!)  
No registered uses  


CallbackType: `OnCreatedColonyGroup`  
=======  
Method type: System.Action<ColonyGroup>  
Registered callbacks: 2  
0.	'disable_some_science' -> 'Science.ScienceManager+Callbacks.OnCreatedColonyGroup'   
1.	'spread_cheatstate' -> 'ColonyGroup+CheatCallbacks.OnCreatedColonyGroup'   


CallbackType: `OnConstructDiplomacyUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu, Colony>  
No registered uses  


CallbackType: `OnConstructCommandTool`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu, string>  
No registered uses  


CallbackType: `OnConstructColonyOwnerManagementUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager.ConstructColonyManagement'   


CallbackType: `OnConstructBannerPlacementUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager+BannerPlacementCallbacks.OnConstructBannerPlacementUI'   


CallbackType: `OnConstructNPCContextMenu`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu, NPC.NPCBase>  
Registered callbacks: 1  
0.	'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnConstructNPCContextMenu' -> 'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnConstructNPCContextMenu'   


CallbackType: `OnConstructBannerClickedUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu, BlockEntities.Implementations.BannerTracker.Banner>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager.ConstructBannerClicked'   


CallbackType: `OnHandleColonySelected`  
=======  
Method type: System.Action<NetworkUI.ButtonPressCallbackData, ColonyID>  
Result of the colony selection menu  
Registered callbacks: 2  
0.	'handle_builtin' -> 'NetworkUI.NetworkMenuManager.HandleSelectedColonyBuiltin'   
1.	'selected_outpost_parent' -> 'NetworkUI.NetworkMenuManager+BannerPlacementCallbacks.OnHandleColonySelected'   


CallbackType: `OnPlayerSelectedTypePopup`  
=======  
Method type: System.Action<Players.Player, ushort, Newtonsoft.Json.Linq.JObject>  
Result of the item selection menu  
Registered callbacks: 1  
0.	'traderule' -> 'NetworkUI.NetworkMenuManager.HandleSelectedTypePopup'   


CallbackType: `OnPlayerSelectedTypePopupCancel`  
=======  
Method type: System.Action<Players.Player, Newtonsoft.Json.Linq.JObject>  
No registered uses  


CallbackType: `OnSaveWorldMisc`  
=======  
Method type: System.Action<Newtonsoft.Json.Linq.JObject>  
called on autosave/quit, node is the json that'll be saved to {world}/world.json  
Registered callbacks: 2  
0.	'save_transports' -> 'Transport.TransportManager+Callbacks.OnSaveWorldMisc'   
1.	'savenpcid' -> 'NPC.NPCTracker+Callbacks.OnSaveWorldMisc'   


CallbackType: `OnLoadWorldMisc`  
=======  
Method type: System.Action<Newtonsoft.Json.Linq.JObject>  
called in AfterItemTypesDefined, node is the json that was saved aerlier ({world}/world.json)  
Registered callbacks: 4  
0.	'load_elevators' -> 'Transport.Elevator.ElevatorTransport+Callbacks.OnLoadWorldMisc'   
1.	'load_gliders' -> 'Transport.Glider+Callbacks.OnLoadWorldMisc'   
2.	'load_rails' -> 'Transport.Rail.RailTransport+Callbacks.OnLoadWorldMisc'   
3.	'loadnpcid' -> 'NPC.NPCTracker+Callbacks.OnLoadWorldMisc'   


CallbackType: `OnConstructColonyStartSettingsUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager.ConstructColonyStartSettings'   


CallbackType: `OnConstructOutpostStartSettingsUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager+CallbackConsumers.OnConstructOutpostStartSettingsUI'   


CallbackType: `OnSendingStatisticsData`  
=======  
Method type: System.Action<Statistics.StatisticsManager>  
Called every time the client requests statistics data;  
include your type definitions every time, so the player can select them  
if the requested key matches your given key, include your desired data that corresponds with the requested time period  
Registered callbacks: 1  
0.	'base' -> 'Statistics.StatisticModCallbacks.OnSendingStatisticsData' index: -1  


CallbackType: `OnGatherStatisticsData`  
=======  
Method type: System.Action<Colony, int, int>  
Called with the colony and stats timeperiod index every time those stats were gathered  
First integer is the period index; 0, 1 or 2 by default  
Second integer is the time between updates for this periods (10, 40 or 240 seconds by default)  
No registered uses  


CallbackType: `OnGatherGroupStatisticsData`  
=======  
Method type: System.Action<ColonyGroup, int, int>  
No registered uses  


CallbackType: `OnLoadModJSONFiles`  
=======  
Method type: System.Action<System.Collections.Generic.List<ModLoader.LoadModJSONFileContext>>  
Registered callbacks: 1  
0.	'pipliz.jsonfilescallbacks' -> 'ModLoader+LoadModJSONFileCallback.OnLoadModJSONFiles'   


CallbackType: `OnPlayerRemovedFromColony`  
=======  
Method type: System.Action<Players.Player, ColonyGroup>  
Registered callbacks: 1  
0.	'removeuimarkers' -> 'ColonyTracker+Callbacks.OnPlayerRemovedFromColony'   


CallbackType: `OnPlayerAddedToColony`  
=======  
Method type: System.Action<Players.Player, ColonyGroup>  
Registered callbacks: 1  
0.	'spread_cheatstate' -> 'ColonyGroup+CheatCallbacks.OnPlayerAddedToColony'   


CallbackType: `OnLoadingImages`  
=======  
Method type: System.Action<System.Collections.Generic.Dictionary<string, string>>  
No registered uses  


CallbackType: `OnRegisterUpgrades`  
=======  
Method type: System.Action<Assets.ColonyPointUpgrades.UpgradesManager>  
Registered callbacks: 1  
0.	'register_upgradeautoload' -> 'Assets.ColonyPointUpgrades.UpgradesManager+CallbacksA.OnRegisterUpgrades'   


CallbackType: `OnConstructPointUpgradesMenu`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu>  
Registered callbacks: 1  
0.	'Assets.UIGeneration.PointsUpgrades.OnConstructPointUpgradesMenu' -> 'Assets.UIGeneration.PointsUpgrades.OnConstructPointUpgradesMenu'   


CallbackType: `OnConstructColonyManageJobsUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu, Colony>  
Registered callbacks: 1  
0.	'Assets.UIGeneration.ColonyManageJobs.OnConstructColonyManageJobsUI' -> 'Assets.UIGeneration.ColonyManageJobs.OnConstructColonyManageJobsUI'   


CallbackType: `OnPlayerEditedNetworkSliderInt`  
=======  
Method type: System.Action<NetworkUI.SliderIntEditCallbackData>  
Registered callbacks: 2  
0.	'Assets.UIGeneration.ColonyManageJobs.OnPlayerEditedNetworkSliderInt' -> 'Assets.UIGeneration.ColonyManageJobs.OnPlayerEditedNetworkSliderInt'   
1.	'NetworkUI.NetworkMenuManager+ToolshopCallbacks.OnPlayerEditedNetworkSliderInt' -> 'NetworkUI.NetworkMenuManager+ToolshopCallbacks.OnPlayerEditedNetworkSliderInt'   


CallbackType: `RegisterNotificationLoaders`  
=======  
Method type: System.Action<System.Collections.Generic.Dictionary<string, Notifications.NotificationManager.NotificationLoader>>  
Registered callbacks: 3  
0.	'Notifications.NPCDeathNotification+Callbacks.RegisterNotificationLoaders' -> 'Notifications.NPCDeathNotification+Callbacks.RegisterNotificationLoaders'   
1.	'Notifications.ResearchCompletedNotification+Callbacks.RegisterNotificationLoaders' -> 'Notifications.ResearchCompletedNotification+Callbacks.RegisterNotificationLoaders'   
2.	'Notifications.SiegeModeNotification+Callbacks.RegisterNotificationLoaders' -> 'Notifications.SiegeModeNotification+Callbacks.RegisterNotificationLoaders'   


CallbackType: `OnRecalculateThreatLevel`  
=======  
Method type: System.Action<ColonyGroup>  
Registered callbacks: 6  
0.	'add_failsafe' -> 'BlockEntities.Implementations.Failsafes+Callbacks.OnRecalculateThreatLevel'   
1.	'add_lockboxes' -> 'BlockEntities.Implementations.Lockboxes+Callbacks.OnRecalculateThreatLevel'   
2.	'add_monsterstatues' -> 'BlockEntities.Implementations.MonsterStatues+Callbacks.OnRecalculateThreatLevel'   
3.	'add_sanctified_lockboxes' -> 'BlockEntities.Implementations.SanctifiedLockboxes+Callbacks.OnRecalculateThreatLevel'   
4.	'check_npc_count' -> 'Difficulty.ColonyThreatLevel+Callbacks2.OnRecalculateThreatLevel'   
5.	'defaultThreat' -> 'Difficulty.ColonyThreatLevel+Callbacks.OnRecalculateThreatLevel'   


CallbackType: `OnGatherMonsterParsers`  
=======  
Method type: System.Action<System.Collections.Generic.Dictionary<NPC.NPCType, System.Func<Saving.WorldDB.MonsterData, Monsters.IMonster>>>  
Registered callbacks: 1  
0.	'Monsters.MonsterSpawner+Callbacks.OnGatherMonsterParsers' -> 'Monsters.MonsterSpawner+Callbacks.OnGatherMonsterParsers'   


CallbackType: `OnRecalculatePointCapacity`  
=======  
Method type: System.Action<ColonyGroup.PointCapacityData>  
Registered callbacks: 1  
0.	'add_lockboxes' -> 'BlockEntities.Implementations.Lockboxes+Callbacks.OnRecalculatePointCapacity'   


CallbackType: `OnRecalculateSanctifiedPointCapacity`  
=======  
Method type: System.Action<ColonyGroup.SanctifiedPointCapacityData>  
Registered callbacks: 2  
0.	'add_failsafe' -> 'BlockEntities.Implementations.Failsafes+Callbacks.OnRecalculateSanctifiedPointCapacity'   
1.	'add_sanctified_lockboxes' -> 'BlockEntities.Implementations.SanctifiedLockboxes+Callbacks.OnRecalculateSanctifiedPointCapacity'   


CallbackType: `OnInventorySelectionChanged`  
=======  
Method type: System.Action<Inventory.InventorySelectionContext>  
Registered callbacks: 2  
0.	'BlockEntities.Implementations.Astrolabe+Callbacks.OnInventorySelectionChanged' -> 'BlockEntities.Implementations.Astrolabe+Callbacks.OnInventorySelectionChanged'   
1.	'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnInventorySelectionChanged' -> 'NetworkUI.NetworkMenuManager+NPCMenuCallbacks.OnInventorySelectionChanged'   


CallbackType: `OnPlayerAttachedToVehicle`  
=======  
Method type: System.Action<Players.Player, MeshedObjects.MeshedVehicleDescription>  
Registered callbacks: 1  
0.	'Transport.TransportManager+Callbacks.OnPlayerAttachedToVehicle' -> 'Transport.TransportManager+Callbacks.OnPlayerAttachedToVehicle'   


CallbackType: `OnPlayerDetachedFromVehicle`  
=======  
Method type: System.Action<Players.Player, MeshedObjects.MeshedVehicleDescription>  
Registered callbacks: 1  
0.	'Transport.TransportManager+Callbacks.OnPlayerDetachedFromVehicle' -> 'Transport.TransportManager+Callbacks.OnPlayerDetachedFromVehicle'   


CallbackType: `OnGenerateNPCName`  
=======  
Method type: System.Action<NPC.NPCNames.NamingContext>  
Registered callbacks: 1  
0.	'NPC.NPCNames.OnGenerateNPCName' -> 'NPC.NPCNames.OnGenerateNPCName'   


CallbackType: `OnEndReadOnly`  
=======  
Method type: System.Action  
Registered callbacks: 3  
0.	'AI.PathingManager+ExecuteManager+Callbacks1.OnEndReadOnly' -> 'AI.PathingManager+ExecuteManager+Callbacks1.OnEndReadOnly'   
1.	'Saving.SaveManager+Callbacks.OnEndReadOnly' -> 'Saving.SaveManager+Callbacks.OnEndReadOnly'   
2.	'TerrainGeneration2.TerrainGenerator2ModManager.OnEndReadOnly' -> 'TerrainGeneration2.TerrainGenerator2ModManager.OnEndReadOnly'   


CallbackType: `OnStartReadOnly`  
=======  
Method type: System.Action  
Registered callbacks: 3  
0.	'AI.PathingManager+ExecuteManager+Callbacks1.OnStartReadOnly' -> 'AI.PathingManager+ExecuteManager+Callbacks1.OnStartReadOnly'   
1.	'Saving.SaveManager+Callbacks.OnStartReadOnly' -> 'Saving.SaveManager+Callbacks.OnStartReadOnly'   
2.	'TerrainGeneration2.TerrainGenerator2ModManager.OnStartReadOnly' -> 'TerrainGeneration2.TerrainGenerator2ModManager.OnStartReadOnly'   


CallbackType: `OnStartMainthread`  
=======  
Method type: System.Action  
No registered uses  


CallbackType: `OnEndMainthread`  
=======  
Method type: System.Action  
Registered callbacks: 1  
0.	'TerrainGeneration2.TerrainGenerator2ModManager.OnEndMainthread' -> 'TerrainGeneration2.TerrainGenerator2ModManager.OnEndMainthread'   


CallbackType: `OnConstructInventoryManageColonyUI`  
=======  
Method type: System.Action<Players.Player, NetworkUI.NetworkMenu, System.ValueTuple<NetworkUI.Items.Table, NetworkUI.Items.Table>>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager+CallbackConsumers.OnConstructInventoryManageColonyUI'   


CallbackType: `OnConstructColonyRecruitmentUI`  
=======  
Method type: System.Action<Players.Player, Newtonsoft.Json.Linq.JObject, System.Collections.Generic.List<NetworkUI.IItem>>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager+CallbackConsumers.OnConstructColonyRecruitmentUI'   


CallbackType: `OnConstructColonySettingsUI`  
=======  
Method type: System.Action<Players.Player, Newtonsoft.Json.Linq.JObject, System.Collections.Generic.List<NetworkUI.IItem>>  
Registered callbacks: 1  
0.	'pipliz.buildbase' -> 'NetworkUI.NetworkMenuManager+CallbackConsumers.OnConstructColonySettingsUI'   


CallbackType: `OnRegisteringEntityManagers`  
=======  
Method type: System.Action<BlockEntities.IEntityManager[]>  
No registered uses  


