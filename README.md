### blackfriday
---
https://github.com/russross/blackfriday

```go
output := blackfriday.MarkdownBasic(input)

output := blackfriday.MarkdownCommon(input)

output := blackfriday.Run(input)

output := blackfriday.Run(input, blackfriday.WithNoExtensions())

import (
  "github.com/microcosm-cc/bluemonday"
  "gopkg.in/russross/blackfriday.v2"
)

unsafe := blackfriday.Run(input)
html := bluemonday.UGCPolicy().SanitizeBytes(unsafe)

func getTrue() bool {
  return true
}

p := bluemonday.UGCPolicy()
p.AllowAttrs("class").Matching(regexp.MustCompile("^language-[a-zA-Z0-9]+$")).OnElements("code")
html := p.SanitizeBytes(unsafe)


```

```
go get -u gopkg.in/russross/blackfriday.v2
go get github.com/russross/blackfriday-tool
```

```
```


