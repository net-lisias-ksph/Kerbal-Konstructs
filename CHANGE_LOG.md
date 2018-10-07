# Kerbal Konstructs :: Change Log

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
