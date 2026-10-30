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
single quote ('\\''),  
and backslash ('\\\\').  

Go also includes the ++ and -- operators to increment and decrement the value of a variable.  
Unlike Java, C++, and several other languages, Go requires these operators to appear after the variable.
```go
var z int = 10
z++ // ok
++z  // syntax error, does not compile
```
Value Overflow:  
Adding one to a variable set to the maximum value for a type returns the minimum value for the type,  
and subtracting one from the minimum returns the maximum.  
Be careful when writing code; don’t assume that z + 1 is always greater than z and z - 1 is always less than z.
```go
var x uint = 0
z--
fmt.Println(z) // prints 18446744073709551615
z++
fmt.Println(z) // prints 0
```
If you do want to write numerical computing applications in Go, use the third-party Gonum package.  
It takes advantage of complex numbers and provides useful libraries for things like  
linear algebra, matrices, integration, graphs, and statistics.  
Other languages have better numerical computing support,  
but Go’s focus on software engineering might be an advantage for larger projects.  





