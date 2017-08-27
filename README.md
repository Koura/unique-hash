# unique-hash

Useful for saving to
```javascript
import uniqueHash from "unique-hash"
let url = "https://www.npmjs.com/package/unique-hash"

uniqueHash(url)
//>> output 

uniqueHash(url)
//>> output

uniqueHash(url,{
 prepend:"prepend",
 append:"append",
 appendDate:"appendDate",
 hash:"hash",
 date:new Date(),
 format:"string"
 }))
 //>> output

```

### Parameters

| Parameter | Default | Description |
|------|-----|
| prepend | "" | string to prepend output path  |
| append | "" |string to append output path  |
| appendDate | "" |  string to center between date and hash id  (eg. output `/YYYY/MM/DD/[HERE]/:hashId`) |
| format | "number" | options: "number" or "string" |
| date | n/a | pass in date to append /YYYY/MM/DD to save path |
| hashId | n/a | override the output hashId, useful if you want to use with date.  |
