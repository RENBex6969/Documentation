# Http API

Getting the function of AHS

```lua
-- // This is different than given when bought
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
