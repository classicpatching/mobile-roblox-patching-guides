# mobile-roblox-patching-guides
- **How To Patch**
> [!NOTE]
> You would Need
> apktool m
> roblox apk from 2014-2015
- **app part**
- You Need To Decompile The Apk
- After it's Decompiled you need to search "roblox.com" and choose replace option and replace with your domain I recommend 10 letter - -  - domain
- after that it patched all stuff in classes.dex and strings, rename .obb of roblox to .zip in assets and extract it and open apktool m -- and go to the extracted .obb folders and search all of them for roblox.com and replace with your domain
- go to res and raw then click roblox_settings and replace domains with yours
- find libroblox.so and then go inside of it using apktool m and replace all domains to yours save it
- then compile it back and download
- if you already have web then enjoy
- **web part**
- in your website create a folder /games/list with a button that redirects you to  /games/start?placeid=1&userId=1 and attempts to get - -- info from /game/PlaceLauncher.ashx
- you should see loading screen in your android client now
- Create A /game/PlaceLauncher.ashx with the following code
- ```{

    "jobId":"join",

    "status":2,

    "joinScriptUrl":"http://yourdomain.name/Game/yourjoinscripthere",

    "authenticationUrl":"http://yourdomain.name/Login/Negotiate.ashx",

    "authenticationTicket":null,

    "message":null

    

}```
