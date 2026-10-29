# golang
Learning and Insights of Golang language. Thanks to Google.

A rune literal represents a single Unicode code point and is surrounded by single quotes.  
Unlike many other languages, in Go single quotes and double quotes are not interchangeable.  

Rune literals can be written as  
single Unicode characters ('a'),  
8-bit octal numbers ('\141'),  
8-bit hexadecimal numbers ('\x61'),  
16-bit hexadecimal numbers ('\u0061'), or 
32-bit Unicode numbers ('\U00000061').  
There are also several backslash-escaped rune literals, with the most useful ones being 
newline ('\n'),  
tab ('\t'),  
single quote ('\''),  
and backslash ('\\').  

Go also includes the ++ and -- operators to increment and decrement the value of a variable.  
Unlike Java, C++, and several other languages, Go requires these operators to appear after the variable.

```go
var x int = 10
x++ // ok
++x  // syntax error, does not compile
```

