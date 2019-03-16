### Mesgs

#### Prepare
```json
{
  "/": {
    "$#{field}_is_required": "[$#{field}] is required",
    "Account_No": "Account No.",
    "Password": "Password",
    "Remember_me": "Remember me"
  },
  "/auth": {
    "Log_in": "Log in",
    "register_now_": "register now!"
  }
}
```

#### API
| Method | Example | Remark |
| -- | -- | -- |
| `static get(key, path = SK.getCurrentPath())` | `'Account_No'` -> `'Account No.'` | |
| `static gets(keys, path = SK.getCurrentPath())` | `['Remember_me','Password']` or `'Remember_me♀Password'` -> `'Remember me Password'` | |
| `static load(path = SK.getCurrentPath(), async = true)` | `'/auth'` -> `{"Log_in":"Log in","register_now_":"register now!"}` | |
| `static unload(path)` | | `'/a'` -> will delete /a**/* |