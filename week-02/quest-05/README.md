# Quest 5

### Expanded Key Concepts

#### 1. Working with Runes

- A rune in Go is an alias for `int32` and represents a single Unicode character. This lets Go easily support international text, emojis, and any character beyond the basic ASCII set.[^5][^7][^9][^10][^11][^12]
- To accurately access runes (not just bytes), convert the string to a `[]rune` slice. This is essential because direct indexing a string (`s`) yields a single byte, which may only form part of a character if the text is Unicode.[^1][^3][^5]
- Functions like `FirstRune`, `LastRune`, and `NRune` highlight how to use loops—either `for range` or explicit `[]rune` conversion—to extract specific runes safely and correctly.[^1][^5]


#### 2. Manual String Manipulation

- Go strings are immutable, so every modification creates a new string. Concatenation is done with `+`, or you can build complex strings using `strings.Builder` for efficiency.[^4][^6]
- Checking characters (isupper, islower, isalpha, isnumeric) requires looping through runes and applying conditional comparisons, often referencing their Unicode code ranges. For example, `'A' <= r && r <= 'Z'` tests uppercase, and `'0' <= r && r <= '9'` tests numeric.
- Custom code for indexing or joining strings demonstrates knowledge of loop control, comparison, and efficient assembly of new strings, while maintaining Go’s memory safety.[^6][^13][^14][^4]


#### 3. Base Conversion Functions

- Go encourages building numeric conversions using custom base definition strings, not only traditional bases like binary or hexadecimal. This involves mapping characters to their numeric values and assembling the result digit-by-digit, handling edge cases for validity and uniqueness.[^15][^16][^17][^18][^19]
- For printing to base, negative numbers, and invalid base strings (too short, repeated characters, or forbidden signs like `+` or `-`), code should fail gracefully or print a specified message (`NV`).
- Parsing strings in a given base requires verifying that each rune belongs in the `base` string and using positional arithmetic to reconstruct the integer.[^3][^17][^15]

***

### Practical Tips

- Always use `for range` or `[]rune` when iterating character-by-character in a string that might use Unicode (non-ASCII) symbols.
- Be mindful of string immutability! Functions that “change” a string actually return new ones.
- Avoid built-in shortcut functions for these exercises—manual code builds deeper understanding, especially of loops, slices, and conditional logic.
- For base manipulation, rigorously test edge cases, including forbidden or invalid bases, empty input, and strings containing non-base symbols.
- Printing runes and converting between types (`rune` to `string`, `int` to `rune`) are common in output/display functions—practice with `fmt.Printf("%c", r)` and related conversions.

***

### Recommended Resources

- **Strings, Bytes, Runes and Characters in Go (Go Blog)**
Detailed explanations and code samples show the differences between strings, bytes, and runes, and why text handling in Go requires careful attention.[^9]
- **Go by Example: Strings and Runes**
Instantly usable samples of real-world string and rune logic in Go.[^1]
- **Introduction to Runes (dev.to)**
Explains how Go uses runes, best initialization practices, and Unicode awareness.[^10]
- **String Manipulation Fundamentals in Go (CodeSignal)**
A lesson dedicated to hands-on character and string logic without built-in library shortcuts.[^4]
- **How to Get the String in Specified Base in Golang? (TutorialsPoint)**
Shows numeric conversions to and from bases, with guidance for robust and reusable code.[^15]
- **A Comprehensive Guide to Type Casting and Conversions in Go (dev.to)**
Explains proper conversion between all major Go types you encounter in these exercises.[^18]
- **Mastering String Manipulation in Go: Techniques and Best Practices**
Tips on string building and safe manipulation without runaway allocations or bugs.[^6]

***

These topics and resources will enable robust and flexible string and character handling in Go for all your Quest 5 tasks—from extracting runes to advanced base conversions.
<span style="display:none">[^2][^8]</span>

<div style="text-align: center">⁂</div>

[^1]: https://gobyexample.com/strings-and-runes

[^2]: https://www.youtube.com/watch?v=7h9qGwdWlJI

[^3]: https://dev.to/jeseekuya/understanding-runes-in-go-4ie5

[^4]: https://codesignal.com/learn/courses/easy-interview-coding-practice-in-go/lessons/string-manipulation-fundamentals-in-go

[^5]: https://zetcode.com/golang/rune/

[^6]: https://www.codingexplorations.com/blog/mastering-string-manipulation-go

[^7]: https://www.codingexplorations.com/blog/understanding-strings-bytes-and-runes-in-go-advantages-and-disadvantages

[^8]: https://itnext.io/runes-in-go-d676b35d2345

[^9]: https://go.dev/blog/strings

[^10]: https://dev.to/hanapiko/introduction-to-runes-2a7l

[^11]: https://zetcode.com/golang/builtins-rune-type/

[^12]: https://exercism.org/tracks/go/concepts/runes

[^13]: https://labex.io/ru/tutorials/go-how-to-perform-string-operations-in-golang-446137

[^14]: https://yourbasic.org/golang/string-functions-reference-cheat-sheet/

[^15]: https://www.tutorialspoint.com/how-to-get-the-string-in-specified-base-in-golang

[^16]: https://stackoverflow.com/questions/41996761/golang-number-base-conversion

[^17]: https://golang.cafe/blog/golang-string-to-int-conversion-example.html

[^18]: https://dev.to/zakariachahboun/a-comprehensive-guide-to-type-casting-and-conversions-in-go-26di

[^19]: https://blog.stackademic.com/a-beginner-friendly-guide-to-type-conversions-in-golang-d2d3aad51db2

