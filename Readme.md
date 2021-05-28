# Regular expressions

> The regular expression object is used for matching text with a pattern. [Know more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp "MDN Page")

```javascript
// expression between // is regular expression literal
// It is an regular expression
const reg = /Hello/
```

_Javascript function related to regular expression_
| Function | Short Defination |
|-----------|------------------|
|match() | It returns **all matches in an array** else **null** [know more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/match "MDN Page")
| test() | If regular expression matches pattern then it returns **true** else **false** [know more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/test "MDN Page")

---

## Flags

### Flag: i

#### Flag **i** is used search pattern without case sensitivity

Example:
_Without_ **i** _flag_

```javascript
let reg = /hello/
const str = "Hello world"

console.log(reg.test(str))

// OUTPUT -> false
```

Example:
_With_ **i** _flag_

```javascript
let reg = /hello/
const str = "Hello world"

console.log(reg.test(str))

// OUTPUT -> true
```

### Flag: g

#### Flag **g** is used search all matched patterns not just the first matched pattern

Example:
_Without_ **g** _flag_

```javascript
let reg = /hello/
const str = "hello world hello user"

console.log(str.match(reg))

// OUTPUT -> ["hello", index: 0, input: "hello world hello user", groups: undefined]
```

Example:
_With_ **g** _flag_

```javascript
let reg = /hello/g
const str = "hello world hello user"

console.log(str.match(reg))

// OUTPUT -> ["hello", "hello"]
```
