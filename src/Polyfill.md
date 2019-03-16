### Polyfill

#### API
| Method | Example | Remark |
| -- | -- | -- |
| `Array.prototype.skFilter(recursive, filterFunc)` | | |
| `Array.prototype.skRmv(item)` | `[1,2,3].skRmv(2)` -> `[1,3]` | |
| `Array.prototype.skToggle(item)` | `[1,2,3].skToggle(2)` -> `[1,3]`, `[1,3].skToggle(2)` -> `[1,2,3]` | |
| `Array.prototype.skTrans(recursive, transFunc)` | | |
| `Number.prototype.skCurrencyFmt(fraction)` | `(-123456.789).skCurrencyFmt(2)` -> `'-123,456.79'` | |
| `Object.prototype.skFilter(recursive, filterFunc)` | | |
| `Object.prototype.skTrans(recursive, transFunc)` | | |
| `Object.prototype.skVal(str, val)` | | like `$.val()` |
| `Object.prototype.skVals()` | `{a: {x: 1}, b: {y: 2}}.skVals()` -> `[{x: 1}, {y: 2}]` | |
| `String.prototype.skBlank()` | `' '.skBlank()` -> `true`, `''.skBlank()` -> `true` | |
| `String.prototype.skCurrencyFmt(fraction)` | `'987654.321'.skCurrencyFmt(2)` -> `'987,654.32'` | |
| `String.prototype.skEmpty()` | `' '.skEmpty()` -> `false`, `''.skEmpty()` -> `true` | |
| `String.prototype.skFmt(o)` | `'My $name {is} $#{name}, i {am from $#{city}'.skFmt({name: 'ShaneKing', city: 'China'})` -> `'My $name {is} ShaneKing, i {am from China'` | |
| `String.prototype.skFmtArr(array)` | `'My $name $#{is} $1, i am$ from $2'.skFmtArr(['ShaneKing', 'China'])` -> `'My $name $#{is} ShaneKing, i am$ from China'` | |