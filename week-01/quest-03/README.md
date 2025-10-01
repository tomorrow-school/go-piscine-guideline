
# Quest 3

To complete QUEST 03 in Go piscine, you should understand pointers, basic arithmetic, string manipulation, string-to-integer conversion, and reverse sorting slices. Here’s a guideline covering core skills and helpful resources.

***

### Main Skills and Sections

- **Pointers (Go Pointers):** Passing and dereferencing single, double, and triple pointers, and mutating referenced values.
- **String operations:** Iterating through strings (rune vs byte), reversing, counting characters.
- **Implementing atoi:** Converting strings to numbers without standard libraries, validity checks, and handling signs.
- **Sorting:** Building primitive slice sort algorithms for ascending order.
- **z01 package:** Used for printable character output (e.g., PrintRune for formatted strings).

***

### Materials and Advice

| Topic | Link or Resource |
| :-- | :-- |
| Go pointers | [Go Pointers — A Tour of Go](https://tour.golang.org/moretypes/1), [Go Spec: Pointer_types](https://golang.org/ref/spec#Pointer_types) |
| String operations | [Go by Example — Strings](https://gobyexample.com/strings), [Go Runerune](https://tour.golang.org/basics/11) |
| Iterating runes | [Go strings and runes](https://blog.golang.org/strings) |
| Implementing atoi | [strconv.Atoi source](https://golang.org/pkg/strconv/#Atoi), [Go by Example: String Parsing](https://gobyexample.com/string-functions) |
| Sorting arrays in Go | [Go sort package (example)](https://gobyexample.com/sorting-slices), [Slice in place algorithms](https://yourbasic.org/golang/slice-reverse/) |
| Using z01 | [01-edu/z01 docs](https://pkg.go.dev/github.com/01-edu/z01) |
| Solutions, templates | [piscine-go solutions](https://github.com/ealhayki/piscine-go), [October45/piscine-go](https://github.com/October45/piscine-go) |


***

### Quick Recommendations by Task

| Task | Skills/Templates | Tips |
| :-- | :-- | :-- |
| pointone | Pointer to int | Pass by reference: *n = 1 |
| ultimatepointone | Triple pointer | Recursively dereference: ***n = 1 |
| divmod/ultimatedivmod | Arithmetic, pointers | Division, modulo with ref passing |
| printstr | String, z01.PrintRune | Iterate over runes, print out |
| strlen | Rune counting | Use `range s`, only runes! |
| swap | Pointer swapping | temp := *a, *a = *b, *b = temp |
| strrev | Rune iteration, slices | Build slice, reverse, reconstruct |
| basicatoi/basicatoi2/atoi | String parsing | Iterate over chars, manage validity/sign |
| sortintegertable | In-place slice sort | Implement bubble/selection/basic logic |


***

### Practical Tips

- Don’t be afraid to experiment with multi-level dereferencing, but keep code readable.
- For strings, use `range` and rune mapping for full Unicode support.
- For atoi, return zero for invalid input and handle plus/minus only at string start.
- For sorting, bubble/selection sort or any basic loop is fine—don’t use built-in sort.
- Use z01.PrintRune for consistent character output formatting.
- Test functions on edge cases (empty strings, single chars, exotic Unicode, large numbers).

***

### Where to Find Example Solutions

- [piscine-go repository with challenge folders and templates](https://github.com/ealhayki/piscine-go).
- [October45/piscine-go](https://github.com/October45/piscine-go) — comparative open-source templates for 01-edu piscine.
- z01 package spec: [pkg.go.dev z01 package](https://pkg.go.dev/github.com/01-edu/z01).

***

This guideline will cover both theory and practice for QUEST 03, providing key materials and best practices for every level (pointers to manual sorting).

***

