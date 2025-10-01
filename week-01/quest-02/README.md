

# Quest 2

To complete QUEST 02 tasks in Go piscine, you’ll need a solid understanding of arithmetic, iteration, recursion, character output, and working with Go’s standard libraries and third-party package z01 for correct printing. Here’s a guideline and a set of materials for practical and theoretical mastery.

***

### Key Skills for QUEST 02

- Go basics: declaring functions, loops, conditions, slices, working with numbers and strings.
- Using custom packages: importing and using third-party libraries (like z01).
- Generating combinations: nested loops and recursive combination generators.
- Formatted output: correct character and number printing.
- Debugging and reading problem statements (constraints, format requirements).

***

### Key Materials for a Fast Start

| Skill/Theme | Resource |
| :-- | :-- |
| Go basics \& syntax | [A Tour of Go](https://tour.golang.org/), [Go by Example](https://gobyexample.com/) |
| Working with numbers/loops | [Learn Go: for/if/func](https://gobyexample.com/for) |
| Using z01 | [z01 package docs](https://pkg.go.dev/github.com/01-edu/z01) |
| Combination generation | [StackOverflow — combinations in Go](https://stackoverflow.com/questions/30226438/generate-combinations-in-go), [printcombn video](https://www.youtube.com/watch?v=_B54KZTjlKU) |
| Review solutions | [piscine-go repositories](https://github.com/ealhayki/piscine-go) |


***

### Recommendations by Task

| Task | Skills/Tools | Tips |
| :-- | :-- | :-- |
| printdigits | Number loops, fmt/z01.PrintRune | Use z01 for stepwise character output |
| isnegative | Condition, chars, function | if-else and z01.PrintRune('T')/'F' |
| printcomb | Nested loops, conditions (i<j<k), output | Don't print ", " after last comb |
| printcomb2 | Nested loops 0-99, output with separator | Same—no trailing ", " |
| printnbr | Number handling, recursion | Print digits char-by-char, no strconv/int64 |
| printcombn | Recursive n-digit combos | Ensure uniqueness, use arrays/slices |


***

### Best Practices

- Always read the output format carefully. Automated tests are sensitive to spaces and punctuation.
- Test edge cases: 0, negative numbers, max values.
- Build a “simple” version first, then generalize the algorithm.
- Prefer z01.PrintRune for character output for consistent formatting.
- For printcomb/printcombn, it’s important to separate the recursive generation from printing.

***

### Where to Review Solutions

- [piscine-go on GitHub](https://github.com/ealhayki/piscine-go) — task breakdowns with comments.
- Video walkthroughs, e.g. printcombn: [print_combn piscine school 42 YouTube].
- Task descriptions from public mirrors: [printcomb — 01-edu public subjects].
- Documentation [github.com/01-edu/z01] and hands-on examples at [pkg.go.dev].

***

This guideline helps navigate typical QUEST 02 tasks, accelerates learning with links to best practices and external reviews, and helps avoid common mistakes with output and combination logic.

***

