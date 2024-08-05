# MultiBlox
 Utility to remove Roblox singleton event so you can run multiple instances of Roblox.  

 I made this for my own use because bloxstrap stopped supporting the multi instance feature.  

 And running older version of bloxstrap was starting to become problematic.. 

## Download
Get the latest release here: [Releases](https://github.com/rasp8erries/multiblox-cs/releases/latest)

## Usage
- Run the "MultiBlox.exe" 
- Administrator privledges are required (select "Yes" when prompted) 
- That's it! Will find existing AND future Roblox instances. 
- If you have problems running it see [Issues](#issues) below. 

![MultiBlox Success](/images/multiblox-success-v1.0.4.png)

## How it works

This Multiblox utility terminates two components of RobloxPlayerBeta.exe (the roblox app) that prevent opening multiple instances of Roblox.

Multiblox will appear in the task tray (beside the system clock and can be closed by right clicking and selecting Exit). In order to continue opening new instancnces of Roblox, Multiblox needs to be running. Closing it will not cause any problems for copies of Roblox that are already open.

Here it is in action with 4 Roblox alts on same computer. 

![example-usage-1](/images/example-usage-1.png)

## Why Admin Required
Admin privileges are required in order to query for the handles of another process (Roblox). 

This is why when you run MultiBlox.exe it will first issue the UAC prompt in order to elevate permissions. 

Otherwise, this will popup when you run MultiBlox. 

![uac-prompt](/images/uac-prompt.png) 

So just click Yes to this to continue. 

## <a name="reqs"></a>Requirements
- Windows Only
- .Net Runtime v8 
  - Get it here: [.Net 8.0](https://aka.ms/dotnet-core-applaunch?framework=Microsoft.NETCore.App&framework_version=8.0.0&arch=x64&rid=win10-x64)

## <a name="issues"></a>Issues
### Nothing Opens
You probably need to download/install [.Net Runtime 8.0](https://aka.ms/dotnet-core-applaunch?framework=Microsoft.NETCore.App&framework_version=8.0.0&arch=x64&rid=win10-x64).

### Security Warnings
If you get a Windows Security warning similar to the below, don't be alarmed. Its only happening because I am not a "known publisher" and this app is access system management stuff in order to watch for new Roblox processes. 

![ms-sec-1](/images/ms-security-1.png)![ms-sec-2](/images/ms-security-2.png) 

