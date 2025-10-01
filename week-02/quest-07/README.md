# Quest 7

Quest 7 focuses on creating and manipulating slices (dynamic arrays) and strings in Go, with a set of tasks that will build a solid understanding of Go’s basics for collection handling, splitting, joining, and numerical base conversions.

***

### Key Concepts

#### 1. Slice Creation and Manipulation: `AppendRange` \& `MakeRange`

- Slices in Go are dynamic arrays. The exercises show two common ways to generate slices from numeric ranges.[^1][^2]
    - `AppendRange`: Typically uses repeated `append()` calls in a loop to build up a slice.
    - `MakeRange`: Uses array literals (`[]int{}`) and index assignment instead of `append` or `make`.
- You’ll learn to handle nil returns on invalid input and work around slice creation limitations.


#### 2. String Joining and Splitting: `ConcatParams`, `SplitWhiteSpaces`, `Split`

- Go strings can be joined (`ConcatParams`) by looping over slices and assembling the final result with a separator, or efficiently with `strings.Join` (practice with and without helpers).[^3][^4]
- Splitting (`SplitWhiteSpaces`, `Split`) usually involves the `strings.Split` or advanced manual parsing to separate by custom delimiters (space, tab, newline, or custom string).[^5][^6][^7]
- Practice converting between slice and string formats, crucial for many CLI and parsing tasks.


#### 3. String Slice Printing: `PrintWordsTables`

- A simple but important Go pattern: printing each element of a string slice on its own line. This strengthens your understanding of loop-control and output.[^2]


#### 4. Base Conversion: `ConvertBase`

- Learn to convert numbers represented as strings from any base to another, by:
    - Parsing the string number to an integer using the source base, often with `strconv.ParseInt` or manual logic.[^8][^9][^10][^11]
    - Constructing a new string representation in the target base by repeatedly dividing and assembling digits.
    - Handling edge cases, valid bases, and result formatting.

***

### Recommended Learning Resources

- **Go by Example: Slices**
Demonstrates all major slice operations, initialization, appending, and iteration.[^2]
- **Creating a Go slice without make (StackOverflow)**
Q\&A describing alternate slice creation methods without the `make` keyword.[^1]
- **String Manipulation Fundamentals in Go (CodeSignal)**
Exercises and explanations for joining, splitting, and printing slices and strings.[^4]
- **How to Split a String in Golang (Educative, GeeksforGeeks, etc.)**
Multiple methods for splitting by delimiters including custom logic.[^12][^6][^7][^5]
- **Golang String To Int Conversion Example (golang.cafe)**
Practical code for converting string to numbers in any base, including Unicode and error handling.[^8]
- **String to int conversion in Golang (Scalent.io)**
Deep dive into `strconv.Atoi` and `strconv.ParseInt` for base conversions.[^9]
- **Mastering String Manipulation in Go: Techniques and Best Practices**
Covers efficient building and transformation of strings and slices.[^3]

***

### Practical Tips

- Prefer `append()` for dynamic slice growth, but learn to use array literals or index assignment for fixed-size slices where `make`/`append` are restricted.
- Manual splitting and joining of strings is great practice for parsing, while using `strings.Split`/`Join` efficiently in production code.[^7][^5]
- Be mindful of error-prone cases: empty inputs, invalid base digits, or numeric conversions with unexpected content.
- For conversion between bases, understand each required step and test with a range of bases and input types for correctness.

***

These patterns and resources will make you confident in handling Go slices and strings for real-world data processing, CLI tools, and algorithm challenges.
<span style="display:none">[^13][^14][^15][^16][^17][^18][^19][^20][^21][^22]</span>

<div style="text-align: center">⁂</div>

[^1]: https://stackoverflow.com/questions/29361377/creating-a-go-slice-without-make

[^2]: https://gobyexample.com/slices

[^3]: https://www.codingexplorations.com/blog/mastering-string-manipulation-go

[^4]: https://codesignal.com/learn/courses/easy-interview-coding-practice-in-go/lessons/string-manipulation-fundamentals-in-go

[^5]: https://www.educative.io/answers/how-to-split-a-string-in-golang

[^6]: https://leapcell.io/blog/how-to-split-strings-in-go

[^7]: https://gosamples.dev/split-string/

[^8]: https://golang.cafe/blog/golang-string-to-int-conversion-example.html

[^9]: https://www.scalent.io/golang/string-to-integer-conversion-in-golang/

[^10]: https://sentry.io/answers/converting-a-string-to-an-integer-in-go/

[^11]: https://metaschool.so/articles/golang-string-to-integer/

[^12]: https://www.geeksforgeeks.org/go-language/how-to-split-a-string-in-golang/

[^13]: https://stackoverflow.com/questions/25543520/declare-slice-or-make-slice

[^14]: https://dev.to/freakynit/using-new-instead-of-make-to-create-slice-17bl

[^15]: https://dev.to/sai7xp/isolating-go-slices-how-to-create-independent-slices-from-an-array-safely-3n1p

[^16]: https://www.w3schools.com/go/go_slices.php

[^17]: https://www.reddit.com/r/golang/comments/16v8yqd/just_started_learning_go_im_confused_about_using/

[^18]: https://stackoverflow.com/questions/4278430/convert-string-to-integer-type-in-go

[^19]: https://forum.golangbridge.org/t/using-make-during-slice-creation/12033

[^20]: https://go.dev/tour/moretypes/13

[^21]: https://purpleschool.ru/knowledge-base/article/split

[^22]: https://stackoverflow.com/questions/71183439/how-can-i-split-a-string-by-the-character

