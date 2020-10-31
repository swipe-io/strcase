# strcase
[![Godoc Reference](https://godoc.org/github.com/swipe-io/strcase?status.svg)](http://godoc.org/github.com/swipe-io/strcase)
[![Build Status](https://travis-ci.org/swipe-io/strcase.svg)](https://travis-ci.org/swipe-io/strcase)
[![Coverage](http://gocover.io/_badge/github.com/swipe-io/strcase?0)](http://gocover.io/github.com/swipe-io/strcase)
[![Go Report Card](https://goreportcard.com/badge/github.com/swipe-io/strcase)](https://goreportcard.com/report/github.com/swipe-io/strcase)

strcase is a go package for converting string case to various cases (e.g. [snake case](https://en.wikipedia.org/wiki/Snake_case) or [camel case](https://en.wikipedia.org/wiki/CamelCase)) to see the full conversion table below.

## Example

```go
s := "AnyKind of_string"
```

| Function                                  | Result               |
|-------------------------------------------|----------------------|
| `ToSnake(s)`                              | `any_kind_of_string` |
| `ToSnakeWithIgnore(s, '.')`               | `any_kind.of_string` |
| `ToScreamingSnake(s)`                     | `ANY_KIND_OF_STRING` |
| `ToKebab(s)`                              | `any-kind-of-string` |
| `ToScreamingKebab(s)`                     | `ANY-KIND-OF-STRING` |
| `ToDelimited(s, '.')`                     | `any.kind.of.string` |
| `ToScreamingDelimited(s, '.', '', true)`  | `ANY.KIND.OF.STRING` |
| `ToScreamingDelimited(s, '.', ' ', true)` | `ANY.KIND OF.STRING` |
| `ToCamel(s)`                              | `AnyKindOfString`    |
| `ToLowerCamel(s)`                         | `anyKindOfString`    |

## Install

```bash
go get -u github.com/swipe-io/strcase
```


## Origin library

iancoleman [strcase](https://github.com/iancoleman/strcase)