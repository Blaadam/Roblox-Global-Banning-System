# Roblox-Global-Banning-System

The Roblox Global Banning System (RGBS) is a system developed by [blaadam](https://www.roblox.com/users/5557366/profile) as a part of a initiative to combat exploiters and other individuals under one hub.

---

### How To Use:
To use RGBS in your own game, please follow the following steps:
- Enable **HttpsService**
- Enable LoadStringEnabled in **ServerScriptService**
- Insert the following code into a server script in ServerScriptService in your own game:
```
local urlToFind = "https://raw.githubusercontent.com/Blaadam/Roblox-Global-Banning-System/main/main.lua" -- **Ensure that this is the raw code**

local httpsService = game:GetService("HttpService")
local getCode = httpsService:GetAsync(urlToFind, true)
local code = loadstring(getCode)
code()
```
