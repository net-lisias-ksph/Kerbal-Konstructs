# Kerbal Konstructs :: Change Log

* 2019-0210: 1.4.5.60 (GER-Space) for KSP 1.4. PRE-RELEASE
	+ changes
			- API for building spanwed event
* 2019-0206: 1.4.5.59 (GER-Space) for KSP 1.4.
	+ Changes
	+ for Players
		- fixed AnimateOnSunrise static module. (switches day/night cycle)
	+ for Modders
			- Added new community textures by Damon
			- added texture tileing option in the Advanced Texture StaticModule
			- made impact resistence configurable ind model config
			- fix a spelling error in the model variant config
			- added a button in the editor that exports all bases (sorted by group) as .tar files into the KerbalKonstructs\ExportedInstances folder  (use winrar or 7-zip) this makes sharing of your own creations a lot easier.
* 2019-0123: 1.4.5.56 (GER-Space) for KSP 1.4.
	+ Changes
		- bugFix for GPP (related to anomalies)
		- added a new tool-bar icon
		- added a universal launchpoint static
		- dynamic static groups for saveGame persistant statics are no longer visible in the statics-editor
* 2019-0123: 1.4.5.54 (GER-Space) for KSP 1.4.
	+ Fix the bug from the latest version.
* 2019-0122: 1.4.5.53 (GER-Space) for KSP 1.4.
	+ editor: make the Squad anomalies visible again
* 2019-0122: 1.4.5.52 (GER-Space) for KSP 1.4.
	+ Fix a crash when ResearchBodies is installed.
* 2019-0120: 1.4.5.51 (GER-Space) for KSP 1.4.
	+ Changes
		- The LaunchSites in the KSP LaunchSite selector are now sorted: 1. KSC 2. Alphabetical order of all KK Launch sites 3. M.H. Launch sites. (the second part is now what is getting sorted. the overall order is nothing I can change.
		- Renaming a launch site in the KK-editor will no longer produce exceptions in other parts of the mod and will propagate properly into the game.
		- fixed an exception when a launchsite is no longer existing withing a saved game.
* 2019-0120: 1.4.5.50 (GER-Space) for KSP 1.4.
	+ Changes
		- Remove orphaned RemoteTech GroundStations when RT support is enabled. This was only be a problem, when you edit GroundStation within a savegame.
		- added 7 Builtin GroupCenters, that are hard linked to POI in Kerbin. KSC, KSC2, Island Airfield, Pyramids, Desert LS, Woomerang LS.
		- Fixed the GrassColor editor.
		- Fixed a problem with the AnimateOnSunRise module (Buildings should turn off the lights more reliable)
		- more verbose error messages in the AnimateOnSunRise module. This sould help modders with setting up thier buildings
* 2019-0109: 1.4.5.47 (GER-Space) for KSP 1.4.
	+ Changes:
		- Less crashing when a PQSMapDecal Map is missing
		- use the active Vessels physics Settings for calculation of the loading range of buildings: fixes: #130
		- minimal improvements of loading time on scene switches
* 2018-1218: 1.4.5.46 (GER-Space) for KSP 1.4.
	+ less crashes when a .cfg could not be loaded
* 2018-1217: 1.4.5.45 (GER-Space) for KSP 1.4.
	+ Changes for players:
		- career games: display the right recovery percentege on the screen.
		- don't reveal hidden bases on the map view
		- enforcement of vessel size, part count and weight for custom launchsites.
		- some suprprise that is fitting for the end of the year.
	+ changes for modders:
			- you can define enforcement of vessel size, part count and weight for custom launchsites. 0 equals unlimited
			- you can define variants of your buildings and they are switchable in the editor.
	+ general improvements
			- dynamic spawning of buildings, when you are near the physical loading range. this will save memory, for unused bases.
			- Despawn of buildings, when you are out of range.
* 2018-1106: 1.4.5.31 (GER-Space) for KSP 1.4.
	+ for players
		- you can now create waypoints to the LaunchSites on the mapview
		- fixed some annoying bugs, that prevented sometimes the launch of vessels
		- the spacecenter camera can focus on bases that are not on the Homeworld.
		- tried to implement some material sharing, so statics can be drawn in batches.
		- The camera in the spacecenter scene should now produce less graphic errors
		- the KK launchsite-selector in the editor shows launchsite type.
	+ for modders
			- increased the accuracy of movement of statics
			- Three new statics from the KSC under the Tanks category to place
* 2018-1114: 1.3.9.31 (GER-Space) for KSP 0.7.3
	+ for players
		- you can now create waypoints to the LaunchSites on the mapview
		- fixed some annoying bugs, that prevented sometimes the launch of vessels
		- the spacecenter camera can focus on bases that are not on the Homeworld.
		- tried to implement some material sharing, so statics can be drawn in batches.
		- The camera in the spacecenter scene should now produce less graphic errors
		- the KK launchsite-selector in the editor shows launchsite type.
	+ for modders
			- increased the accuracy of movement of statics
* 2018-1106: 1.4.5.26 (GER-Space) for KSP 1.5.1 PRE-RELEASE
	+ increased the accuracy of movement of statics
* 2018-1028: 1.4.5.24 (GER-Space) for KSP 1.5.1
	+ For modders
	+ new GroupCenter objects. These are the center of a group and define everything
	+ new config file format: now everything is relative to a GroupCenter
	+ group editing: You can move and clone an entire group of statics
	+ automatic group assignment of newly created statics
	+ new editor gizmo support for object movement
	+ you can switch the reference system in the editor with the "F" key
	+ Improved GrasColor support. (predefined colors, texture replacement)
	+ added AnimateOnTrigger StaticModule
	+ For all
			- better support for Sigma Dimensions. As soon statics are loaded with the new config format, everything will stay in place.
			- speeded up the loading of Kerbin-Side Remastered statics (20x faster)
			- general prformance improvements
			- automatic conversion of old configs to new format
			- Statics should now always load outside the VesselLoading range. (try to fix multiplayer and physic-range altering mods)
			- fixed some bugs regarding the MH-Expansion LaunchSite Selector. (still not 100% Bug-Free)
* 2018-0812: 1.4.5.4 (GER-Space) for KSP 1.4.
	+ for everyone
		- Changes the tooltip of the recovery bases to the FacilityName or the LaunchSite name
		- new Squad static to place: The lights of the desert runway (one section of them) are now a standalone static which can be placed anywhere (when expansion is installed)
		- the Mapview of the recovery bases now caches its contents, which is now slightly more resource friendly.
	+ for modders
			- Added API call for placing statics: PlaceStatic()
			- Added a trigger-CallBack StaticModule, where mods can register CallBack functions when a part enters the trigger collider.
			- Added API calls to register collider callback functions (OnEnter, OnStay and OnExit)
			- Statics: Editor: You can use the statics editor after you used the PQSMap editor
			- Statics: Editor: You can now enter most values with less problems and they are applied after pressing <Enter>
	+ internal
			- Changed the Water-Floating StaticModule to use the CallBack StaticModule, so I have less duplicate code.
* 2018-0807: 1.4.5.2 (GER-Space) for KSP 1.4.
	+ New Features
		- You can visualize all Recovery Bases in the mapvew, so its easier to aim for one. (even the new Recovery-Only ones)
		- The both dishes for of the lv1 tracking station are now animated
	+ BugFixes
		- Put the sound cube collider into a different layer, so it doesn't interfere with KSP 1.4.X anymore.
	+ For Modders
			- New Feature: static objects can be savegame persistent. (only in the game they are spawned, and saved in the persistance .sfs
			- New Feature: a "reduced feature set" statics editor, which can be called through a API call.
			- New Feature: Some API Calls for adding and removing Statics, which a saved in the persistance sfs
			- New Feature: StaticModels can be hidden from the normal editor with isHidden = true in the model .cfg
			- New Feature: New Facility type: RecoveryBase: Make a static a base for vessel recovery. No launchSite needed (think of a SpaceX Barge, you land there, you get 100% return)
			- BugFix: AdracedTexture: Material replacement now works correctly on multiple transforms.
			- Added two water-surface statics. one round, one square. (FBX included)
	+ internal
			- All statics have now a unique ID, that is used when saving and loading persistance information. This speeds up level KK related scene loading times by 50%
* 2018-0504: 1.4.5.0 (GER-Space) for KSP 1.4.4
	+ Changes:
			- Stock Squad buildings now have lower energy bills. (they turn off thier lights during the day)
			- KK building now behave in the SC view and you can no longer click through active GUI windows
			- Added SurfaceWater support for statics
			- added support for material switching (in the AdvancedTexture Static Module)
			- the launchsite selector no longer crashes if you deleted the config of the last used launchsite.
			- Fixes a spelling error in the DishAnimate module (some old configs might break, please update your configs. Its now RotationTransform and not RotationTrasform (missing "n")
			- Fixes a Bug in the PQS Editor. Now the NewInstances Directory is created when savong a PQSMod
			- Made the MobileLaunchPad and Desert Airfield usable as LaunchSites
			- Added the Desert Airfield Statics into the Statics Database as seperate objects
* 2018-0503: 1.4.3.3 (GER-Space) for KSP 1.4.3
	+ Changes:
			- fix wreck spawning on stock buildings
			- less explosing vessels with the PQS editor
			- Set warp to next morning a bit later on Kopernikus planets
* 2018-0501: 1.4.3.2 (GER-Space) for KSP 1.4.3
	+ This is a bugFix release for KSP 1.4.3:
			- MH: Fixed crash when gpoing back to the mainmenue
			- Career: Fixed a crash on the vessel recovery dialog
			- MH: Career: Opened bases now stay open
			- MH: The default launch button are now correctly set and update correctly for sites
* 2018-0429: 1.4.3.1 (GER-Space) for KSP 1.4.
	+ ' Fix .dds texture handling for the advances Texture Module.
* 2018-0321: 1.4.3.0 (GER-Space) for KSP 1.4.
	+ Last Update: 29.4.2018
	+ Support for KSP 1.4.X
			- Added LaunchPad-Smoke support
			- Added support for the Stock-Expansion LaunchSite selector
			- Fixed a bug that prevended a crash during load, when slower computers are used and many mods are installed
			- Vessel spawned on waterlaunchsites are no longer spawned under water
			- KSC2 LaunchSite is usable without any mods (in Career games you have to find it first and open it when you are landed near to it)
			- To make KK more compatible with KSC changing mods, it will no longer ship the assets from Alpha-Ash. These will be moved into Kerbin-Side
			- Errors when saving models should no longer crash KK
* 2018-1105: 1.3.9.24 (GER-Space) for KSP 1.3.1
	+ For modders
	+ new GroupCenter objects. These are the center of a group and define everything
	+ new config file format: now everything is relative to a GroupCenter
	+ group editing: You can move and clone an entire group of statics
	+ automatic group assignment of newly created statics
	+ new editor gizmo support for object movement
	+ you can switch the reference system in the editor with the "F" key
	+ Improved GrasColor support. (predefined colors, texture replacement)
	+ added AnimateOnTrigger StaticModule
	+ For all
			- better support for Sigma Dimensions. As soon statics are loaded with the new config format, everything will stay in place.
			- speeded up the loading of Kerbin-Side Remastered statics (20x faster)
			- general prformance improvements
			- automatic conversion of old configs to new format
			- Statics should now always load outside the VesselLoading range. (try to fix multiplayer and physic-range altering mods)
* 2018-1028: 1.3.9.18 (GER-Space) for KSP 1.3.1 PRE-RELEASE
	+ Added Group Editing and broke everything.
	+ Make a backup before you use this:
			- Backport of the 1.4 code to 1.2.2 and 1.3.1
* 2018-0819: 1.3.9.15 (GER-Space) for KSP 1.3.1 PRE-RELEASE
	+ Editor backport (direct enty of values), fix for MapDecal Editor killing the StaticsEditor
	+ make LV3 Tracking Station Dish available as a static
	+ animate dishes of lV1 & 2 Tracking stations
	+ make the Group Setting avaiable in the MapDecal editor. (currently unused, but will be used in future releases
	+ UUIDs will be created for all Statics (but currently not used)
* 2018-0811: 1.3.9.14 (GER-Space) for KSP 1.3.1
	+ Advanced Textures: Fixed the Material Replacer
	+ Added some Watersurface Assets
	+ Animated the Lv1 tracking station dishes
	+ The MapDecal Parser uses ByteCode Reader for images
* 2018-0503: 1.3.9.12 (GER-Space) for KSP 1.3.1
	+ This is the release as from 03.May 2018 for KSP 1.3.1
	+ Changes:
			- Added LaunchPad Smoke effects
			- Warp to next morning is nor a bit later on Kopernikus planets
			- Added KSC2 support
			- fix: KSC building wrecks are now back again
			- removed statics for Kerbin-Side rematered
			- fix sound support for animations
* 2018-0423: 1.3.9.10 (GER-Space) for KSP 1.3.1
	+ Added sound support for AnimanteOnclick
	+ AninimteOnClick supports now muliple collider objects with the same name.
	+ BugFix: Warp to next morning button is working correctly with Custom Planet packs using kopernikus.
	+ the KSC2 is a builtin base: On career games it is hidden, so you have to get near first and open it up for one credit. No Kerbin-Side needed.
	+ Added smoke effects for Launchpads
	+ the Assets and RoundRidge Base from AlphaAsh are moved to into the Kerbin-Side releae
* 2018-0321: 1.3.9.8 (GER_Space) for KSP 1.3.1
	+ More Bugfixes
		- Rocket LaunchSites might had a bug in the latest release:
		- AutoKouse module does not throu an exception anymore
* 2018-0320: 1.3.9.7 (GER_Space) for KSP 1.3.1
	+ fix crash in the launchsite editor
* 2018-0319: 1.3.9.6 (GER_Space) for KSP 1.3.1
	+ 19.3.2018 1.3.9.6
			- For players
			- BugFix: The last LaunchSite used should not be resetted all the time
			- BugFix: KCT is annoying: repairing it made some bugs visible in the code.
			- BugFix: Default LaunchSies are now set correctly
			- NGS should now work correctly
			- The SpaceCenter view will now show the last LaunchSite used. (you can switch this off in the configs)
			- Most facilities will bring you to the correspondig SC facility scenses when clicked from the SpaceCenter overview.
			- You can have the Keribin-Side and Stock CommNet GroundStations at the same time (config switch in the settings) You don't need to restart KSP to change that behavior
			- Landing Guides reworkd to be more useful and less annoying
			- For modders
			- LaunchSites are now fully usable after placing them. No need to restart KSP to test them.
			- reworked the AutoKourse Static Module. The digit meshes are freely configuable and you can adjust the heading offset.
			- Added a PAPI StaticModule (for Eskandare)
			- KK will redeploy all statics after a GameDatabase reload. (this will Reset your Facilities, so handle with care)
			- Added a DishAnimate Static Module for easy animation of antennas. (They are controlled by the same module as the stock antennas)
			- LaunchSite editor:  You can define the initial angle of the SpaceCenter camera (clockwise from the LaunchSite forward vector)
			- BugFix:The Category Search is now woking again in the models overview
			- the AdvancedTexture Modules allows multiple meshes in a comma seperated list
			- the AdvancedTexture caches the builtin textures for faster loading.
			- AdvancedTexture Module: Addes a BuiltinIndex = <int>, so you can refer to diffrent textures with the same name.
			- Internal
			- changed internal LaunchSite handling. (for easier KSP1.4 migration)
			- BugFix: no more errors in the logfile, when placing Squads buildings.
* 2018-0309: 1.3.0.3 (GER_Space) for KSP 1.3.1
	+ Bugfix: Small error in the mapdecaleditor
	+ BugFix: #66 Fic KTC integration & better player position detection
* 2018-0308: 1.3.0.1 (GER_Space) for KSP 1.3.1
	+ fix the LaunchSite selector windows in the SPH
* 2018-0308: 1.3.0.0 (GER_Space) for KSP 1.3.1
	+ Changes:
		- For players
		- Fixed the facility dublications in the inflight facility manager
		- Some windows generate less memory garbage and should render faster
		- Added a new Merchant facility type. You can trade all defined resources here.
		- FuelTanks are converted to the new Merchant Facility
		- Added a new Storage Facility Type. You can place and retrieve all your resources there
		- Reworked Vessel Recovery: All Open LaunchSites have the same recovery range and factor as the KSC. If you are closer than 2500m to a base you get 100% refund. As balancing all LaunchSiterefunds have been removed, as it didn't make any sense. The old recovery could have lead to situations that recovery at a remote base was worse than at the KSC. Also fixed the display of the recovery window.
		- (experimental )KerbalKonstructs should work better with SigmaDimensions, as now the altitude for most objects is saved in height above terrain. (floating objects at the water surface should stay there.
		- For modders
		- Objects can be now moved and edited outside the visiblility range of the object.
		- StaticModules have now an attribute staticInstance which is automaticly updated when the module is attached to an Static Object.
		- Support for placing and editig PQSMod_MapDecals
		- Added Support to load custom MapDecal image maps (examples in the MapDecalMaps folder)
		- added some helper vectors to visualize the mapdecals area of effect
		- Added a GradColor static module, that will adjust the color or the named meshes to the color of the underground. (and set a new gras texture)
		- You can use builtin Textures with the BUILDIN:/ prefex. (currently used in the GrasColor Module and the AdvancedTexture Module)
		- Added AdvanedTexture StaticModule for replacing textures and shaders on a Static.
		- Added AnimateOnSunRise StaticModule (created by @Li0n-0 )
		- All KSP Assets now come with the GrasColor Module preinstalled
		- Internal
		- complete rework of the LaunchSiteManager and the LaunchSiteSelector GUI. It should render faster and has 300 less lines of Code. It is also better to read.
* 2018-0210: 1.2.0.4 (GER_Space) for KSP 1.3.1
* 2018-0210: 1.2.0.3 (GER_Space) for KSP 1.3.1
	+ Changes:
			- Set the default behavior of the CommNet and RemoteTech support to false.
			- Fixed the facility editor
			- removed unneccesary the calls to the staticModuleUpdate when a object is selected.
			- made the the KerbalKonstricts.UI.StaticsEditorGUI.isOpen() function public, so it can be queried from other mods.
			- Fixed the snap2target and copy/paste position of objects.
			- removed some orphaned code from the editor.
			- small peformace improvements to the statics editor
			- Fixed the offices and research facilities. They now prodoce about 5 science and 5000 credits per kerbal and year, so they are now slightly usefull.
* 2017-1007: 1.2.0.1 (GER_Space) for KSP 1.3.1
	+ recompile for KSP 1.3.1
* 2017-0915: 1.2.0.0 (GER_Space) for KSP 1.3.0
	+ Big Changes:
		- New NavUtils Addon by Whale_2: Runways can now create thier own config so they show up in NavUtils. Kerbin-Side will be updated later to make use of it.
		- The persistence handling changed once again, so all LaunchSites and facilities are closed again, but should now stay open for all players, once they are opened again. please use alt+f12 to refund your closed bases.
	+ Changes for players:
			- the settings for KK are now migrated to KSP settings system
			- Try to implement a bugfix for the loading problem of facility states, that plaques some players.
			- All windows of KK are now only loaded, when they are accessed for the first time. this should save some RAM
			- BugFix: an empty configuration without any additional runways will no longer crash KSP. This should fix some issues RSS & GPP users had.  (1.1.9.7)
			- Recovery of vessels near a KK base should now result in a proper refund of credits. (BugFix for KSP 1.3) (1.1.9.7)
	+ Changes for modders:
			- you can select where the config files for newly placed static go (GameData/NewInstances or GameData/KerbalKonstrucs/NewInstances)
			- You can now switch to the old editor camera mode (in the KK settings). Please don't do this while the KK editor window is open.
			- Models can now use custom shaders. (new setting: useShader = "Name of the Shader") (untested)
			- KK will load and use all shaders, that are in .KSP asset bundles.
			- BugFix: Setting the group from the statics window will no longer delete all objects in range.
			- BugFix: Editor: The Snap to Terrain button now does what it should do.
			- BugFix: The Squad KSC models should now produce less errors when loaded, after new instances are placed by KK
			- BugFix: Squad anomalies will now show up more than only once after an restart of KSP
			- BugFix: Make launchSiteEditor work again. (1.1.9.5)
* 2017-0610: 1.1.0 (GER_Space) for KSP 1.3.0
	+ added more Squad  models (KSC wrecks and animalies) to the preloaded model editor lists
* 2017-0603: 1.0.0b (GER_Space) for KSP 1.3.0
	+ updated .version file
* 2017-0504: 0.9.9.6 (GER_Space) for KSP 1.2.2
	+ Fixed framerate Issues introduced in last release
	+ FlagDecal Module should work on multiple flags per object
* 2017-0502: 0.9.9.5 (GER_Space) for KSP 1.2.2
	+ Changes for Players:
			- CommNet Support: All Antennas are the same strength as the KSC ones
			- RemoteTech Support: The antennas have the Ranges as displayed on the map.
	+ You need to enable the Support each of the setting in the KK mod settings (accessable from the spacecenter menue)
	+ For best gameplay experience, use the latest Kerbin-Side packages (GroundControl or complete)
			- a new KerbalKonstruct Mission Flag by SpannerMonkey
			- less memory garbage creation during gameplay. --> better performance.
	+ Changes for Modders:
			- added dynamic runway markings by whale_2. The model kourseXX will display the corresponding runway number according to its heading.
			- Added new StaticModule: "FlagDecal" This is basicly the same module as for Parts. It sets a texture of a Model to th actual flag.
			- SpannerMonkey contributed a new BillBoard Model, which displays your current MissionFlag
			- Added the KSC facility models to the list of placeable models.
				- isScanable" flag for instances: These objects will show up in anomaly scanners as marks. (setable in the editor)
			- hidden flag for Launchsites: Closed Launchsites are not shown in map or launchsite selector when marked "hidden". You need to go there first and open them
			- When the KK-editor is open, you can select (most) statics under the mousepointer by pressing the "left shift" key.
	+ boring stuff
				- New persistence Layer for savegames
* 2016-1212: 0.9.8.9 (GER_Space) for KSP 1.2.2
	+ Changes:
			- Launchsites: KK will add the KSC to the correct position, if the Homeplanet is altered. also KK will not crash when the home is not named Kerbin.
			- cfg loader: configfiles for unknown bodies are no longer crashing KK.
* 2016-1208: 0.9.8.8 (GER_Space) for KSP 1.2.2
	+ Changes:
			- new statics: added runway markings by whale_2. Thank you!
			- new placed objects are written to: GameData\KerbalKonstructs\NewInstances[modelname]-instances.cfg
			- editor: finer increments when editing objects.
			- editor: used relative directions instead of altering some vectors.
			- editor: added reference vectors
			- editor: orientation uses reference vectors
			- editor: added scaling of objects
			- editor: facilities are now editable for placed objects
			- editor: fixed editing of Kerbin-Side statics
			- cfg file loader: "RadialPosition" can be recalculated, when missing, from RefLatitude/RefLongitude
			- all: enabled some more debug output.
* 2016-1121: 0.9.8.5 (GER_Space) for KSP 1.2.1
	+ Changes:
			- fixed loading of the kosmodrome mod.
			- added a "set Launchsite" Button to the launchsite selector, because I searched always there for one.
			- map: can show waterlaunch sites (toggled via the "other" category)
			- editor: added a waterlaunch category to the launchsite editor
			- editor: added set increment buttons to the statics editor
* 2016-1120: 0.9.8.4 (GER_Space) for KSP 1.2.1
	+ Changes:
			- Much faster startup.
			- KSC(Launchpad&Runway) is now selectable in MapView (again?)
			- A bit more verbose message, when you are out of range of an fuel tank
			- Camera is now resetting after a facitity was selected and the window is closed.
			- Recovering of vessels is now fixed. (Also StageRecovery is working again since last release)
* 2016-1110: 0.9.8.2 (GER_Space) for KSP 1.2.1
	+ No changelog provided
* 2016-0729: 0.9.7.3 (AlphaAsh) for KSP 1.1.3
	+ Internal versioning changes to support newer Contract Configurator versions.
* 2016-0710: 0.9.7.2 (AlphaAsh) for KSP 1.1.3
	+ Updated for KSP 1.1.3.
* 2016-0527: 0.9.7.1 (AlphaAsh) for KSP 1.1.2
	+ Added a center sight to the landing guidance HUD.
	+ Added a glide-slope meter to just under the center sight.
* 2016-0519: 0.9.7.0 (AlphaAsh) for KSP 1.1.2
	+ This is an experimental version. That means it has new features that aren't necessarily finished. It may also mean bugs.
	+ If you don't like experimental features or risk of bugs, then don't update.
	+ Added a new landing guidance feature.
	+ Currently only implemented at Round Range and KSC.
	+ To activate landing guidance, switch on ATC in the Inflight Base Boss when close to one of the bases.
	+ A HowTo for base/static makers for implementing landing guidance will be in the Kerbal Konstructs thread of the KSP forums soon.
	+ Expect more bases with landing guidance when static packs get updated.
	+ This is a first go at it, so expect changes and feedback is welcome.
* 2016-0515: 0.9.6.9_EX (AlphaAsh) for KSP 1.1.2
	+ This is an experimental version. That means it has new features that aren't necessarily finished. It may also mean bugs.
	+ If you don't like experimental features or risk of bugs, then don't update.
	+ Fuel Tank instances can now have three new properties: LqFAlt, OxFAlt, MoFAlt.
	+ They can be acted on/added in a cfg by MM to provide the name of an alternative resource.
	+ Please see the Kerbal Konstructs thread of the KSP forums for more information on how to utilise these properties.
	+ Fuel Tanks now have a x25 and x100 transfer rate for quicker refuels.
* 2016-0513: 0.9.6.8_EX (AlphaAsh) for KSP 1.1.2
	+ This is an experimental version. That means it has new features that aren't necessarily finished.
	+ It may also mean bugs.
	+ If you don't like experimental features or risk of bugs, then don't update.
	+ Added Master Export function to Developer Mode. Use this to do a batch export of ALL instances to KerbalKonstructs/ExportedInstances/Master.
	+ This function doesn't care if an instance is a CustomInstance or not.
	+ The organisation is much tidier in the Master folder than when using the other export functions.
	+ Added a GroupCenter and RefCenter property to instances. If you don't want to wait for Kerbin-Side to update with these, please use the Master Export function and they'll be included in the exported cfgs.
	+ Proceed with caution - advanced stuff for developers only in this version of KK.
* 2016-0509: 0.9.6.7_EX (AlphaAsh) for KSP 1.1.2
	+ This is an experimental version. That means it has new features that aren't necessarily finished.
	+ It may also mean bugs.
	+ If you don't like experimental features or risk of bugs, then don't update.
	+ Tracking station/map view KK bar now has toggles for displaying uplinks, ground comms (hardlines, telecomms etc.) and radar.
	+ Tracking station/map view KK bar now has an occlude toggle, used to switch hiding of icons behind a planet.
	+ Zooming out from a planet, radar and icons will now disappear at a distance.
	+ Please note that new features are usually just aesthetic in an experimental version of KK.
* 2016-0504: 0.9.6.6_EX (AlphaAsh) for KSP 1.1.2
	+ This is an experimental version. That means it has new features that aren't necessarily finished.
	+ It may also mean bugs.
	+ If you don't like experimental features or risk of bugs, then don't update.
	+ Started implementing new features for operational tracking stations.
	+ Uplinks from tracking stations to vessels in orbit of that body are now displayed in the tracking station/map view.
	+ A green line means the station uplink has a lock. A red line means it doesn't.
* 2016-0430: 0.9.6.5 (AlphaAsh) for KSP 1.1.2
	+ Recompiled against KSP 1.1.2.
	+ Sent angry e-mail to TriigerAu and Ted for releasing a new version of KSP right after a release of KK. Again.
	+ No, not really.
* 2016-0430: 0.9.6.4 (AlphaAsh) for KSP 1.1.1
	+ Fixed custom logo and icon pathing for custom launchsites.
	+ Added a tip to the KK KSC app regarding how to access the editor.
	+ Addressed lag caused in Space Center scene when using this app.
	+ Added a disclaimer to the Downlink to make it clearer it's WIP, currently just a toy and no it doesn't work with RemoteTech.
* 2016-0429: 0.9.6.3 (AlphaAsh) for KSP 1.1.1
	+ Recompiled against KSP 1.1.1.
* 2016-0428: 0.9.6.2_HOT (AlphaAsh) for KSP 1.1.1
	+ FPS killing fixed
* 2016-0428: 0.9.6.1 (AlphaAsh) for KSP 1.1
	+ Updates to hooks for KerKonConCon.dll.
	+ If you use Kerbin-Side Jobs contracts you want this for the latest update of that.
* 2016-0426: 0.9.6.0 (AlphaAsh) for KSP 1.1
	+ GUI windows sizes revised to deal with font sizing issues introduced by Unity 5.
	+ Tooltips revised to deal with font sizing issues introduced by Unity 5.
	+ Added model cfg parameter keepConvex. Set this true in your model's cfg if you don't want KK to convert your colliders to concave automatically.
	+ Homeworld no longer hard-coded as Kerbin (for RSS support).
* 2016-0424: 0.9.5.9 (AlphaAsh) for KSP 1.1
	+ Under the hood work for upcoming support of Contract Configurator and RemoteTech.
	+ All KK apps use the same icon in every scene now.
	+ Added some missing icons for KK's Space Center app.
	+ As well as access to the mod's settings, KK's Space Center app now includes some minor previews of upcoming features. Please note some of these may not happen.
	+ Under the hood work for some upcoming features.
	+ This mod includes version checking using
	+ [MiniAVC](http://forum.kerbalspaceprogram.com/threads/79745). If you opt-in, it will use the internet to check whether there is a new version available. Data is only read from the internet and no personal information is sent. For a more comprehensive version checking experience, please download the [KSP-AVC Plugin](http://forum.kerbalspaceprogram.com/threads/79745).
* 2016-0412: 0.9.5.8 (AlphaAsh) for KSP 1.1
	+ Fixed disappearing tracking stations in map view/tracking center.
	+ Fixed Round Range operational facilities not being operational.
* 2016-0403: 0.9.5.7 (AlphaAsh) for KSP 1.1
	+ Fixed a bug where using the launch dialogs at the KSC scene would b0rk up flight results and reverting flights.
	+ Custom bases now log launches and you can see the log in the Base Manager. Please note that the KSC does not keep this log since everyone thinks Gene should do it and he's busy with things like managing contracts... erm, controlling missions. No I don't get it either.
* 2016-0401: 0.9.5.6 (AlphaAsh) for KSP 1.1
	+ Fixed a bug in the GUI code for the Inflight Base Boss causing it to appear blank.
	+ Inflight Base Boss a little more informative when stuff can and can't be done with it.
* 2016-0331: 0.9.5.5 (AlphaAsh) for KSP 1.1
	+ Fixed a bug where the recovery button wouldn't work when at or near a base.
* 2016-0331: 0.9.5.4 (AlphaAsh) for KSP 1.1
	+ Fixed bug in recovery, where KSC wasn't getting cleaned up and funds was continuously increased.
	+ Cleaned up example core static cfgs so that duplication errors aren't logged incorrectly when Round Range is being spawned on game start.
* 2016-0330: 0.9.5.3 (AlphaAsh) for KSP 1.1
	+ This is a test version. If you don't want to test the latest version, then don't update.
	+ This version is compiled against the pre-release version 1.1 of KSP with a few minor code changes for compatibility with API updates. That means there has been no major overhaul of the GUI and other planned improvements that utilise the Unity update.
	+ It does not require module manager anymore. The collider "fix" is applied automatically to all static objects. All static object colliders are set concave and preliminary testing shows that Unity does still support them.
	+ It does seem to work just fine in x64, based on preliminary testing.
* 2016-0222: 0.9.5.2 (AlphaAsh) for KSP 1.0.5
	+ Non-critical update.
	+ Updated MM config to support all statics, regardless of author.
	+ Updated/validated version file.
* 2016-0218: 0.9.5.1 (AlphaAsh) for KSP 1.0.5
	+ This is the interim version that includes the fix for collider issues in KSP 1.0.5.
	+ Credit to Thomas P. and Joshwoo69 for the work on this.
	+ Also included the MM cfg necessary for the fix to be applied by any statics made by me.
	+ Also included the latest version of Module Manager.
* 2016-0218: 0.9.5.0 (AlphaAsh) for KSP 1.0.4
	+ No changelog provided
