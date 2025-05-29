# Http API

Getting the function of AHS

```lua
local Kry = loadstring(game:HttpGet(""))()
```

## Kry.request

```lua
-- Same as request but has AHS
Kry.request({})
```

* Example

Doing a Kry.request on HttpBin/post

```lua
-- // This is different than given when bought
local Kry = loadstring(game:HttpGet(""))()

local HttpService = game:GetService("HttpService")
local response = Kry.request({
    Url = "https://httpbin.org/post",
    Method = "POST",
    Headers = {
        ["Content-Type"] = "application/json"
    },
})

print("Status code:", response.StatusCode)
print("Body:", response.Body)

```

## Kry.HttpGet

```lua
Kry.HttpGet("url") -- basically game.HttpGet but with AHS
```

## Kry.getVersion

Returns the current version of AHS
```
print(Kry.getVersion())
```
