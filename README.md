# Gemgen

Gemgen is a simple library for generating Gemtext.

# Usage
## Installation
```
go get github.com/trebabcock/gemgen
```

## Example
Using gemgem is very easy, if not a little verbose.
```go
func generateGemtext() string {
    buffer := gemgen.Gemtext{}

    buffer.AddHeader("Hello, world")
    buffer.AddLink("gemini://geminispace.info/", "Gemini Search Engine")
    buffer.AddUnformatted("I am unformatted text.")

    return buffer.Buffer
}
```