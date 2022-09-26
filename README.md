# Crashlog-9.26.22

---- Minecraft Crash Report ----
// Uh... Did I do that?

Time: 2022-09-26 16:21:31
Description: Initializing game

net.minecraftforge.fml.ModLoadingException: Forge (forge) encountered an error during the common_setup event phase
§7java.lang.IllegalArgumentException: No delegate exists for value air
	at net.minecraftforge.fml.javafmlmod.FMLModContainer.acceptEvent(FMLModContainer.java:111) ~[javafmllanguage-1.19.2-43.1.1.jar%23215!/:?] {}
	at net.minecraftforge.fml.ModLoader.lambda$postEvent$34(ModLoader.java:306) ~[fmlcore-1.19.2-43.1.1.jar%23214!/:?] {}
	at java.lang.Iterable.forEach(Iterable.java:75) ~[?:?] {re:computing_frames,re:mixin}
	at net.minecraftforge.fml.ModList.forEachModInOrder(ModList.java:225) ~[fmlcore-1.19.2-43.1.1.jar%23214!/:?] {re:mixin}
	at net.minecraftforge.fml.ModLoader.postEvent(ModLoader.java:306) ~[fmlcore-1.19.2-43.1.1.jar%23214!/:?] {}
	at net.minecraftforge.client.ForgeHooksClient.onItemColorsInit(ForgeHooksClient.java:321) ~[forge-1.19.2-43.1.1-universal.jar%23218!/:?] {re:mixin,re:classloading}
	at net.minecraft.client.color.item.ItemColors.m_92683_(ItemColors.java:92) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:mixin,pl:runtimedistcleaner:A,re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.<init>(Minecraft.java:493) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:blueprint.mixins.json:client.MinecraftMixin,pl:mixin:APP:iceberg.mixins.json:MinecraftMixin,pl:mixin:APP:architectury.mixins.json:MixinMinecraft,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.m_239872_(Main.java:176) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:51) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?] {}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.minecraftforge.fml.loading.targets.CommonClientLaunchHandler.lambda$launchService$0(CommonClientLaunchHandler.java:27) ~[fmlloader-1.19.2-43.1.1.jar%2395!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:30) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:53) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:71) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:106) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:77) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) [bootstraplauncher-1.1.2.jar:?] {}
Caused by: java.lang.IllegalArgumentException: No delegate exists for value air
	at net.minecraftforge.registries.ForgeRegistry.lambda$getDelegateOrThrow$5(ForgeRegistry.java:550) ~[forge-1.19.2-43.1.1-universal.jar%23218!/:?] {re:classloading}
	at java.util.Optional.orElseThrow(Optional.java:403) ~[?:?] {re:mixin}
	at net.minecraftforge.registries.ForgeRegistry.getDelegateOrThrow(ForgeRegistry.java:550) ~[forge-1.19.2-43.1.1-universal.jar%23218!/:?] {re:classloading}
	at net.minecraft.client.color.item.ItemColors.m_92689_(ItemColors.java:105) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:mixin,pl:runtimedistcleaner:A,re:classloading,pl:runtimedistcleaner:A}
	at net.minecraftforge.common.ForgeSpawnEggItem$ColorRegisterHandler.lambda$registerSpawnEggColors$1(ForgeSpawnEggItem.java:114) ~[forge-1.19.2-43.1.1-universal.jar%23218!/:?] {re:classloading,pl:eventbus:A}
	at java.util.ArrayList.forEach(ArrayList.java:1511) ~[?:?] {re:computing_frames,re:mixin}
	at net.minecraftforge.common.ForgeSpawnEggItem$ColorRegisterHandler.registerSpawnEggColors(ForgeSpawnEggItem.java:113) ~[forge-1.19.2-43.1.1-universal.jar%23218!/:?] {re:classloading,pl:eventbus:A}
	at net.minecraftforge.common.__ColorRegisterHandler_registerSpawnEggColors_Item.invoke(.dynamic) ~[forge-1.19.2-43.1.1-universal.jar%23218!/:?] {re:classloading,pl:eventbus:B}
	at net.minecraftforge.eventbus.ASMEventHandler.invoke(ASMEventHandler.java:73) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:315) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:296) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.fml.javafmlmod.FMLModContainer.acceptEvent(FMLModContainer.java:107) ~[javafmllanguage-1.19.2-43.1.1.jar%23215!/:?] {}
	... 22 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Render thread
Stacktrace:
	at net.minecraftforge.fml.javafmlmod.FMLModContainer.acceptEvent(FMLModContainer.java:111) ~[javafmllanguage-1.19.2-43.1.1.jar%23215!/:?] {}
	at net.minecraftforge.fml.ModLoader.lambda$postEvent$34(ModLoader.java:306) ~[fmlcore-1.19.2-43.1.1.jar%23214!/:?] {}
	at java.lang.Iterable.forEach(Iterable.java:75) ~[?:?] {re:computing_frames,re:mixin}
	at net.minecraftforge.fml.ModList.forEachModInOrder(ModList.java:225) ~[fmlcore-1.19.2-43.1.1.jar%23214!/:?] {re:mixin}
	at net.minecraftforge.fml.ModLoader.postEvent(ModLoader.java:306) ~[fmlcore-1.19.2-43.1.1.jar%23214!/:?] {}
	at net.minecraftforge.client.ForgeHooksClient.onItemColorsInit(ForgeHooksClient.java:321) ~[forge-1.19.2-43.1.1-universal.jar%23218!/:?] {re:mixin,re:classloading}
	at net.minecraft.client.color.item.ItemColors.m_92683_(ItemColors.java:92) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:mixin,pl:runtimedistcleaner:A,re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.<init>(Minecraft.java:493) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:blueprint.mixins.json:client.MinecraftMixin,pl:mixin:APP:iceberg.mixins.json:MinecraftMixin,pl:mixin:APP:architectury.mixins.json:MixinMinecraft,pl:mixin:A,pl:runtimedistcleaner:A}
-- Initialization --
Details:
	Modules: 
		ADVAPI32.dll:Advanced Windows 32 Base API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		AMSIExt.dll:McAfee Cloud AV ThirdParty Ext:26.3.109 dddedcaa gossamer carrot:McAfee, LLC
		COMCTL32.dll:User Experience Controls Library:6.10 (WinBuild.160101.0800):Microsoft Corporation
		CRYPT32.dll:Crypto API32:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		CRYPTBASE.dll:Base cryptographic API DLL:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		CRYPTSP.dll:Cryptographic Service Provider API:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		ColorAdapterClient.dll:Microsoft Color Adapter Client:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		CoreMessaging.dll:Microsoft CoreMessaging Dll:10.0.19041.746:Microsoft Corporation
		CoreUIComponents.dll:Microsoft Core UI Components Dll:10.0.19041.546:Microsoft Corporation
		DBGHELP.DLL:Windows Image Helper:10.0.19041.867 (WinBuild.160101.0800):Microsoft Corporation
		DEVOBJ.dll:Device Information Set DLL:10.0.19041.1620 (WinBuild.160101.0800):Microsoft Corporation
		DNSAPI.dll:DNS Client API DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		GDI32.dll:GDI Client DLL:10.0.19041.1620 (WinBuild.160101.0800):Microsoft Corporation
		GLU32.dll:OpenGL Utility Library DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		IMM32.DLL:Multi-User Windows IMM32 API Client DLL:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		IPHLPAPI.DLL:IP Helper API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		KERNEL32.DLL:Windows NT BASE API Client DLL:10.0.19041.1741 (WinBuild.160101.0800):Microsoft Corporation
		KERNELBASE.dll:Windows NT BASE API Client DLL:10.0.19041.1741 (WinBuild.160101.0800):Microsoft Corporation
		MMDevApi.dll:MMDevice API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		MSCTF.dll:MSCTF Server DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		NLAapi.dll:Network Location Awareness 2:10.0.19041.1151 (WinBuild.160101.0800):Microsoft Corporation
		NSI.dll:NSI User-mode interface DLL:10.0.19041.610 (WinBuild.160101.0800):Microsoft Corporation
		NTASN1.dll:Microsoft ASN.1 API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		Ole32.dll:Microsoft OLE for Windows:10.0.19041.1320 (WinBuild.160101.0800):Microsoft Corporation
		OleAut32.dll:OLEAUT32.DLL:10.0.19041.985 (WinBuild.160101.0800):Microsoft Corporation
		OpenAL.dll:Main implementation library:1.21.1:
		PROPSYS.dll:Microsoft Property System:7.0.19041.1708 (WinBuild.160101.0800):Microsoft Corporation
		PSAPI.DLL:Process Status Helper:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		Pdh.dll:Windows Performance Data Helper DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		RPCRT4.dll:Remote Procedure Call Runtime:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		SETUPAPI.dll:Windows Setup API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		SHCORE.dll:SHCORE:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		SHELL32.dll:Windows Shell Common Dll:10.0.19041.964 (WinBuild.160101.0800):Microsoft Corporation
		UMPDC.dll
		USER32.dll:Multi-User Windows USER API Client DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		USERENV.dll:Userenv:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		VCRUNTIME140.dll:Microsoft® C Runtime Library:14.29.30139.0 built by: vcwrkspc:Microsoft Corporation
		VERSION.dll:Version Checking and File Installation Libraries:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		WINHTTP.dll:Windows HTTP Services:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		WINMM.dll:MCI API DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		WINSTA.dll:Winstation Library:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		WINTRUST.dll:Microsoft Trust Verification APIs:10.0.19041.1949 (WinBuild.160101.0800):Microsoft Corporation
		WS2_32.dll:Windows Socket 2.0 32-Bit DLL:10.0.19041.1081 (WinBuild.160101.0800):Microsoft Corporation
		WSOCK32.dll:Windows Socket 32-Bit DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		WTSAPI32.dll:Windows Remote Desktop Session Host Server SDK APIs:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		Wldp.dll:Windows Lockdown Policy:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		amsi.dll:Anti-Malware Scan Interface:10.0.19041.1620 (WinBuild.160101.0800):Microsoft Corporation
		apphelp.dll:Application Compatibility Client Library:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		awt.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		bcrypt.dll:Windows Cryptographic Primitives Library:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		bcryptPrimitives.dll:Windows Cryptographic Primitives Library:10.0.19041.1415 (WinBuild.160101.0800):Microsoft Corporation
		cfgmgr32.dll:Configuration Manager DLL:10.0.19041.1620 (WinBuild.160101.0800):Microsoft Corporation
		clbcatq.dll:COM+ Configuration Catalog:2001.12.10941.16384 (WinBuild.160101.0800):Microsoft Corporation
		combase.dll:Microsoft COM for Windows:10.0.19041.1320 (WinBuild.160101.0800):Microsoft Corporation
		cryptnet.dll:Crypto Network Related API:10.0.19041.906 (WinBuild.160101.0800):Microsoft Corporation
		dbgcore.DLL:Windows Core Debugging Helpers:10.0.19041.789 (WinBuild.160101.0800):Microsoft Corporation
		dhcpcsvc.DLL:DHCP Client Service:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		dhcpcsvc6.DLL:DHCPv6 Client:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		dinput8.dll:Microsoft DirectInput:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		drvstore.dll:Driver Store API:10.0.19041.1949 (WinBuild.160101.0800):Microsoft Corporation
		dwmapi.dll:Microsoft Desktop Window Manager API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		dxcore.dll:DXCore:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		fwpuclnt.dll:FWP/IPsec User-Mode API:10.0.19041.1503 (WinBuild.160101.0800):Microsoft Corporation
		gdi32full.dll:GDI Client DLL:10.0.19041.2006 (WinBuild.160101.0800):Microsoft Corporation
		glfw.dll:GLFW 3.4.0 DLL:3.4.0:GLFW
		icm32.dll:Microsoft Color Management Module (CMM):10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		inputhost.dll:InputHost:10.0.19041.1741 (WinBuild.160101.0800):Microsoft Corporation
		java.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		javaw.exe:OpenJDK Platform binary:17.0.3.0:Microsoft
		jemalloc.dll
		jimage.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		jli.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		jna9463530030124658656.dll:JNA native library:6.1.2:Java(TM) Native Access (JNA)
		jsvml.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		jvm.dll:OpenJDK 64-Bit server VM:17.0.3.0:Microsoft
		kernel.appcore.dll:AppModel API Host:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		lwjgl.dll
		lwjgl_opengl.dll
		lwjgl_stb.dll
		management.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		management_ext.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		msasn1.dll:ASN.1 Runtime APIs:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		mscms.dll:Microsoft Color Matching System DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		msvcp140.dll:Microsoft® C Runtime Library:14.29.30139.0 built by: vcwrkspc:Microsoft Corporation
		msvcp_win.dll:Microsoft® C Runtime Library:10.0.19041.789 (WinBuild.160101.0800):Microsoft Corporation
		msvcrt.dll:Windows NT CRT DLL:7.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		mswsock.dll:Microsoft Windows Sockets 2.0 Service Provider:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		napinsp.dll:E-mail Naming Shim Provider:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		ncrypt.dll:Windows NCrypt Router:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		net.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		nio.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		ntdll.dll:NT Layer DLL:10.0.19041.1741 (WinBuild.160101.0800):Microsoft Corporation
		ntmarta.dll:Windows NT MARTA provider:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		nvoglv64.dll:NVIDIA Compatible OpenGL ICD:30.0.15.1295:NVIDIA Corporation
		nvspcap64.dll:NVIDIA Game Proxy:3.18.0.102:NVIDIA Corporation
		opengl32.dll:OpenGL Client DLL:10.0.19041.1806 (WinBuild.160101.0800):Microsoft Corporation
		perfos.dll:Windows System Performance Objects DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		pnrpnsp.dll:PNRP Name Space Provider:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		powrprof.dll:Power Profile Helper DLL:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		profapi.dll:User Profile Basic API:10.0.19041.844 (WinBuild.160101.0800):Microsoft Corporation
		rasadhlp.dll:Remote Access AutoDial Helper:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		rsaenh.dll:Microsoft Enhanced Cryptographic Provider:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		sechost.dll:Host for SCM/SDDL/LSA Lookup APIs:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		shlwapi.dll:Shell Light-weight Utility Library:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		sunmscapi.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		textinputframework.dll:"TextInputFramework.DYNLINK":10.0.19041.1806 (WinBuild.160101.0800):Microsoft Corporation
		ucrtbase.dll:Microsoft® C Runtime Library:10.0.19041.789 (WinBuild.160101.0800):Microsoft Corporation
		uxtheme.dll:Microsoft UxTheme Library:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		vcruntime140_1.dll:Microsoft® C Runtime Library:14.29.30139.0 built by: vcwrkspc:Microsoft Corporation
		verify.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
		win32u.dll:Win32u:10.0.19041.2006 (WinBuild.160101.0800):Microsoft Corporation
		windows.storage.dll:Microsoft WinRT Storage API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		winrnr.dll:LDAP RnR Provider DLL:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		wintypes.dll:Windows Base Types DLL:10.0.19041.1320 (WinBuild.160101.0800):Microsoft Corporation
		wshbth.dll:Windows Sockets Helper DLL:10.0.19041.546 (WinBuild.160101.0800):Microsoft Corporation
		xinput1_4.dll:Microsoft Common Controller API:10.0.19041.1 (WinBuild.160101.0800):Microsoft Corporation
		zip.dll:OpenJDK Platform binary:17.0.3.0:Microsoft
Stacktrace:
	at net.minecraft.client.main.Main.m_239872_(Main.java:176) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:51) ~[client-1.19.2-20220805.130853-srg.jar%23213!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?] {}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.minecraftforge.fml.loading.targets.CommonClientLaunchHandler.lambda$launchService$0(CommonClientLaunchHandler.java:27) ~[fmlloader-1.19.2-43.1.1.jar%2395!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:30) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:53) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:71) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:106) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:77) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) [bootstraplauncher-1.1.2.jar:?] {}


-- System Details --
Details:
	Minecraft Version: 1.19.2
	Minecraft Version ID: 1.19.2
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 17.0.3, Microsoft
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), Microsoft
	Memory: 2843954024 bytes (2712 MiB) / 4429185024 bytes (4224 MiB) up to 12884901888 bytes (12288 MiB)
	CPUs: 8
	Processor Vendor: GenuineIntel
	Processor Name: Intel(R) Core(TM) i7-9700 CPU @ 3.00GHz
	Identifier: Intel64 Family 6 Model 158 Stepping 13
	Microarchitecture: Coffee Lake
	Frequency (GHz): 3.00
	Number of physical packages: 1
	Number of physical CPUs: 8
	Number of logical CPUs: 8
	Graphics card #0 name: NVIDIA GeForce GTX 1660 Ti
	Graphics card #0 vendor: NVIDIA (0x10de)
	Graphics card #0 VRAM (MB): 4095.00
	Graphics card #0 deviceId: 0x2182
	Graphics card #0 versionInfo: DriverVersion=30.0.15.1295
	Memory slot #0 capacity (MB): 16384.00
	Memory slot #0 clockSpeed (GHz): 2.67
	Memory slot #0 type: DDR4
	Virtual memory max (MB): 27521.88
	Virtual memory used (MB): 14915.59
	Swap memory total (MB): 11264.00
	Swap memory used (MB): 353.50
	JVM Flags: 9 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx12G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	Launched Version: 1.19.2-forge-43.1.1
	Backend library: LWJGL version 3.3.1 build 7
	Backend API: NVIDIA GeForce GTX 1660 Ti/PCIe/SSE2 GL version 3.2.0 NVIDIA 512.95, NVIDIA Corporation
	Window size: <not initialized>
	GL Caps: Using framebuffer using OpenGL 3.2
	GL debug messages: 
	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'forge'
	Type: Client (map_client.txt)
	CPU: 8x Intel(R) Core(TM) i7-9700 CPU @ 3.00GHz
	OptiFine Version: OptiFine_1.19.2_HD_U_H9
	OptiFine Build: 20220820-230904
	Render Distance Chunks: 16
	Mipmaps: 4
	Anisotropic Filtering: 1
	Antialiasing: 0
	Multitexture: false
	Shaders: BSL_v8.1.03.zip
	OpenGlVersion: 3.2.0 NVIDIA 512.95
	OpenGlRenderer: NVIDIA GeForce GTX 1660 Ti/PCIe/SSE2
	OpenGlVendor: NVIDIA Corporation
	CpuCount: 8
	ModLauncher: 10.0.8+10.0.8+main.0ef7e830
	ModLauncher launch target: forgeclient
	ModLauncher naming: srg
	ModLauncher services: 
		mixin-0.8.5.jar mixin PLUGINSERVICE 
		eventbus-6.0.3.jar eventbus PLUGINSERVICE 
		fmlloader-1.19.2-43.1.1.jar slf4jfixer PLUGINSERVICE 
		fmlloader-1.19.2-43.1.1.jar object_holder_definalize PLUGINSERVICE 
		fmlloader-1.19.2-43.1.1.jar runtime_enum_extender PLUGINSERVICE 
		fmlloader-1.19.2-43.1.1.jar capability_token_subclass PLUGINSERVICE 
		accesstransformers-8.0.4.jar accesstransformer PLUGINSERVICE 
		fmlloader-1.19.2-43.1.1.jar runtimedistcleaner PLUGINSERVICE 
		modlauncher-10.0.8.jar mixin TRANSFORMATIONSERVICE 
		modlauncher-10.0.8.jar OptiFine TRANSFORMATIONSERVICE 
		modlauncher-10.0.8.jar fml TRANSFORMATIONSERVICE 
	FML Language Providers: 
		minecraft@1.0
		lowcodefml@null
		javafml@null
	Mod List: 
		ancient_manuscripts-1.0.2-1.19.2.jar              |Ancient Manuscripts           |ancient_manuscripts           |1.0.2-1.19.2        |COMMON_SET|Manifest: NOSIGNATURE
		jei-1.19.2-forge-11.3.0.262.jar                   |Just Enough Items             |jei                           |11.3.0.262          |COMMON_SET|Manifest: NOSIGNATURE
		The_Graveyard_1.12_(FORGE)_for_1.19.2.jar         |The Graveyard                 |graveyard                     |1.12                |COMMON_SET|Manifest: NOSIGNATURE
		AttributeFix-Forge-1.19.2-17.1.2.jar              |AttributeFix                  |attributefix                  |17.1.2              |COMMON_SET|Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		ForgeEndertech-1.19.2-10.0.5.0-build.0599.jar     |ForgeEndertech                |forgeendertech                |10.0.5.0            |COMMON_SET|Manifest: NOSIGNATURE
		AdFinders-1.19.2-8.0.4.0-build.0626.jar           |Advanced Finders              |adfinders                     |8.0.4.0             |COMMON_SET|Manifest: NOSIGNATURE
		piglinproliferation-1.19-1.0.0.jar                |Piglin Proliferation          |piglinproliferation           |1.19-1.0.0          |COMMON_SET|Manifest: NOSIGNATURE
		Clumps-forge-1.19.2-9.0.0+11.jar                  |Clumps                        |clumps                        |9.0.0+11            |COMMON_SET|Manifest: NOSIGNATURE
		XaerosWorldMap_1.27.0_Forge_1.19.1.jar            |Xaero's World Map             |xaeroworldmap                 |1.27.0              |COMMON_SET|Manifest: NOSIGNATURE
		shutupexperimentalsettings-1.0.5.jar              |Shutup Experimental Settings! |shutupexperimentalsettings    |1.0.5               |COMMON_SET|Manifest: NOSIGNATURE
		Prism-1.19.1-1.0.2.jar                            |Prism                         |prism                         |1.0.2               |COMMON_SET|Manifest: NOSIGNATURE
		SereneSeasons-1.19.2-8.1.0.21.jar                 |Serene Seasons                |sereneseasons                 |0.0NONE             |COMMON_SET|Manifest: NOSIGNATURE
		configured-1.5.8-1.19.jar                         |Configured                    |configured                    |1.5.8               |COMMON_SET|Manifest: NOSIGNATURE
		ItemBorders-1.19.1-1.2.0.jar                      |Item Borders                  |itemborders                   |1.2.0               |COMMON_SET|Manifest: NOSIGNATURE
		Bookshelf-Forge-1.19.2-16.1.5.jar                 |Bookshelf                     |bookshelf                     |16.1.5              |COMMON_SET|Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		BagOfHolding-v4.1.2-1.19.2-Forge.jar              |Bag Of Holding                |bagofholding                  |4.1.2               |COMMON_SET|Manifest: 9a:09:85:98:65:c4:8c:11:c5:49:f6:d6:33:23:39:df:8d:b4:ff:92:84:b8:bd:a5:83:9f:ac:7f:2a:d1:4b:6a
		consistency_plus-forge-0.5.1+1.19.2.jar           |Consistency Plus              |consistency_plus              |0.5.1+1.19.2        |COMMON_SET|Manifest: NOSIGNATURE
		jeed-1.19.2-1.17.jar                              |Just Enough Effect Description|jeed                          |1.19.2-1.17         |COMMON_SET|Manifest: NOSIGNATURE
		HopoBetterUnderwaterRuins-1.19-1.1.jar            |HopoBetterUnderwaterRuins     |hopour                        |1.0.9               |COMMON_SET|Manifest: NOSIGNATURE
		blueprint-1.19-6.0.7.jar                          |Blueprint                     |blueprint                     |6.0.7               |COMMON_SET|Manifest: NOSIGNATURE
		BetterThanMending-1.7.2.jar                       |BetterThanMending             |betterthanmending             |1.7.2               |COMMON_SET|Manifest: NOSIGNATURE
		frozenup-2.0.0-forge.jar                          |Frozen Up                     |frozenup                      |2.0.0-forge         |COMMON_SET|Manifest: NOSIGNATURE
		3dskinlayers-forge-1.5.2-mc1.19.1.jar             |3dSkinLayers                  |skinlayers3d                  |1.5.2               |COMMON_SET|Manifest: NOSIGNATURE
		forge-1.19.2-43.1.1-universal.jar                 |Forge                         |forge                         |43.1.1              |COMMON_SET|Manifest: 84:ce:76:e8:45:35:e4:0e:63:86:df:47:59:80:0f:67:6c:c1:5f:6e:5f:4d:b3:54:47:1a:9f:7f:ed:5e:f2:90
		supplementaries-1.19.2-2.2.3.jar                  |Supplementaries               |supplementaries               |1.19.2-2.2.3        |COMMON_SET|Manifest: NOSIGNATURE
		neapolitan-1.19-4.0.1.jar                         |Neapolitan                    |neapolitan                    |4.0.1               |COMMON_SET|Manifest: NOSIGNATURE
		EquipmentCompare-1.19.1-1.3.1.jar                 |Equipment Compare             |equipmentcompare              |1.3.1               |COMMON_SET|Manifest: NOSIGNATURE
		client-1.19.2-20220805.130853-srg.jar             |Minecraft                     |minecraft                     |1.19.2              |COMMON_SET|Manifest: a1:d4:5e:04:4f:d3:d6:e0:7b:37:97:cf:77:b0:de:ad:4a:47:ce:8c:96:49:5f:0a:cf:8c:ae:b2:6d:4b:8a:3f
		mcw-bridges-2.0.4-mc1.19.2forge.jar               |Macaw's Bridges               |mcwbridges                    |2.0.4               |COMMON_SET|Manifest: NOSIGNATURE
		FarmersDelight-1.19-1.2.0.jar                     |Farmer's Delight              |farmersdelight                |1.19-1.2.0          |COMMON_SET|Manifest: NOSIGNATURE
		TerraBlender-forge-1.19.2-2.0.1.127.jar           |TerraBlender                  |terrablender                  |2.0.1.127           |COMMON_SET|Manifest: NOSIGNATURE
		moonlight-1.19.2-2.0.29.jar                       |Moonlight Library             |moonlight                     |1.19.2-2.0.29       |COMMON_SET|Manifest: NOSIGNATURE
		MouseTweaks-forge-mc1.19-2.23.jar                 |Mouse Tweaks                  |mousetweaks                   |2.23                |COMMON_SET|Manifest: NOSIGNATURE
		totw_additions-1.2.3-1.19.x-forge.jar             |Towers of the Wild: Additions |totw_additions                |1.2.3               |COMMON_SET|Manifest: NOSIGNATURE
		ToolStats-Forge-1.19.2-12.0.2.jar                 |ToolStats                     |toolstats                     |12.0.2              |COMMON_SET|Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		Jade-1.19.1-forge-8.2.2.jar                       |Jade                          |jade                          |8.2.2               |COMMON_SET|Manifest: NOSIGNATURE
		geode-1.1.2-1.19.2.jar                            |Geode+                        |geode                         |1.1.2+1.19.2        |COMMON_SET|Manifest: NOSIGNATURE
		additionaladditions-5.0.2.jar                     |Additional Additions          |additionaladditions           |5.0.2               |COMMON_SET|Manifest: NOSIGNATURE
		HopoBetterRuinedPortals-1.19-1.3.2b.jar           |HopoBetterRuinedPortals       |hoporp                        |1.3.1               |COMMON_SET|Manifest: NOSIGNATURE
		AdLods-1.19.2-7.0.4.0-build.0599.jar              |Large Ore Deposits            |adlods                        |7.0.4.0             |COMMON_SET|Manifest: NOSIGNATURE
		NethersDelight-1.19-3.0.jar                       |Nether's Delight              |nethersdelight                |1.19-3.0            |COMMON_SET|Manifest: NOSIGNATURE
		CNB-1.19-1.4.0.jar                                |Creatures and Beasts          |cnb                           |1.4.0               |COMMON_SET|Manifest: NOSIGNATURE
		Iceberg-1.19-1.0.46.jar                           |Iceberg                       |iceberg                       |1.0.46              |COMMON_SET|Manifest: NOSIGNATURE
		curios-forge-1.19.2-5.1.1.0.jar                   |Curios API                    |curios                        |1.19.2-5.1.1.0      |COMMON_SET|Manifest: NOSIGNATURE
		Patchouli-1.19.2-76.jar                           |Patchouli                     |patchouli                     |1.19.2-76           |COMMON_SET|Manifest: NOSIGNATURE
		LegendaryTooltips-1.19.1-1.3.0.jar                |Legendary Tooltips            |legendarytooltips             |1.3.0               |COMMON_SET|Manifest: NOSIGNATURE
		ecologics-forge-1.19.2-2.1.10.jar                 |Ecologics                     |ecologics                     |2.1.10              |COMMON_SET|Manifest: NOSIGNATURE
		stonecutter_recipe_tags-4.0.0+1.19.9b8d04c.forge.j|Stonecutter Recipe Tags       |stonecutter_recipe_tags       |4.0.0+1.19.9b8d04c.f|COMMON_SET|Manifest: NOSIGNATURE
		Lexicon-1.19.2-(v.1.2.0).jar                      |Lexicon                       |lexicon                       |1.2.0               |COMMON_SET|Manifest: NOSIGNATURE
		AutoRegLib-1.8-54.jar                             |AutoRegLib                    |autoreglib                    |1.8-54              |COMMON_SET|Manifest: NOSIGNATURE
		Quark-3.3-371.jar                                 |Quark                         |quark                         |3.3-371             |COMMON_SET|Manifest: NOSIGNATURE
		abnormals_delight-1.19-4.0.0.jar                  |Abnormals Delight             |abnormals_delight             |4.0.0               |COMMON_SET|Manifest: NOSIGNATURE
		ToughAsNails-1.19-8.0.0.78.jar                    |Tough As Nails                |toughasnails                  |0.0NONE             |COMMON_SET|Manifest: NOSIGNATURE
		Dreamland-forge-1.19.2-1.2.0.2.jar                |Dreamland                     |dreamland                     |1.2.0.2             |COMMON_SET|Manifest: NOSIGNATURE
		backpacked-2.1.10-1.19.jar                        |Backpacked                    |backpacked                    |2.1.10              |COMMON_SET|Manifest: NOSIGNATURE
		raised-forge-1.19.2-1.1.2.jar                     |Raised                        |raised                        |1.1.2               |COMMON_SET|Manifest: NOSIGNATURE
		sapience-1.19-1.1.0.jar                           |Sapience                      |sapience                      |1.1.0               |COMMON_SET|Manifest: NOSIGNATURE
		architectury-6.2.46-forge.jar                     |Architectury                  |architectury                  |6.2.46              |COMMON_SET|Manifest: NOSIGNATURE
		PuzzlesLib-v4.3.4-1.19.2-Forge.jar                |Puzzles Lib                   |puzzleslib                    |4.3.4               |COMMON_SET|Manifest: 9a:09:85:98:65:c4:8c:11:c5:49:f6:d6:33:23:39:df:8d:b4:ff:92:84:b8:bd:a5:83:9f:ac:7f:2a:d1:4b:6a
		charmofundying-forge-6.0.0+1.19.2.jar             |Charm of Undying              |charmofundying                |6.0.0+1.19.2        |COMMON_SET|Manifest: NOSIGNATURE
		AdChimneys-1.19.2-9.1.5.0-build.0599.jar          |Advanced Chimneys             |adchimneys                    |9.1.5.0             |COMMON_SET|Manifest: NOSIGNATURE
		FastLeafDecay-30.jar                              |FastLeafDecay                 |fastleafdecay                 |30                  |COMMON_SET|Manifest: NOSIGNATURE
		Delightful-1.19-2.6.jar                           |Delightful                    |delightful                    |2.6                 |COMMON_SET|Manifest: NOSIGNATURE
		CosmeticArmorReworked-1.19.2-v1.jar               |CosmeticArmorReworked         |cosmeticarmorreworked         |1.19.2-v1           |COMMON_SET|Manifest: 5e:ed:25:99:e4:44:14:c0:dd:89:c1:a9:4c:10:b5:0d:e4:b1:52:50:45:82:13:d8:d0:32:89:67:56:57:01:53
		geckolib-forge-1.19-3.1.21.jar                    |GeckoLib                      |geckolib3                     |3.1.21              |COMMON_SET|Manifest: NOSIGNATURE
		winteroverhaul-2.0.1.jar                          |Winter Overhaul               |winteroverhaul                |2.0.1               |COMMON_SET|Manifest: NOSIGNATURE
		creeperoverhaul-2.0.4-forge.jar                   |Creeper Overhaul              |creeperoverhaul               |1.0.0               |COMMON_SET|Manifest: NOSIGNATURE
		BetterAdvancements-1.19.2-0.2.2.142.jar           |Better Advancements           |betteradvancements            |0.2.2.142           |COMMON_SET|Manifest: NOSIGNATURE
	Crash Report UUID: fc09b63b-f30e-4d5f-80c8-18ecec2e3d9d
	FML: 43.1
	Forge: net.minecraftforge:43.1.1
