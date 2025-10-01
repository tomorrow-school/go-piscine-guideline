# Quest 4

To solve QUEST 04 tasks in this block, you’ll need knowledge of recursion, iteration, basic search algorithms, arithmetic cycles, prime searching, and classic puzzles like the "eight queens problem". Here’s a guideline by topic and approach for each problem.

***

### General Skills and Knowledge

- **Iterative and recursive loops:** For Factorial and Power — be able to implement both kinds of solutions without standard functions.
- **Fibonacci:** Classic recursion, pay special attention to base cases.
- **Prime number analysis:** Optimization—only check divisibility up to square root.
- **Backtracking puzzles:** Eight queens is a placement puzzle; avoid conflicts by row, column, and diagonal.
- **Finding square roots:** Simple brute-force, integer-only.
- **Finding next prime:** Iteratively search upward, checking primality.

***

### Key Materials and Sources

| Topic | Resource or Link |
| :-- | :-- |
| Factorial algorithms | [Recursion explained: video](https://www.youtube.com/watch?v=4W6CTp1eBe0) |
| Iteration and recursion Go | [Go by Example: Recursion](https://gobyexample.com/recursion), [Go loops](https://gobyexample.com/for) |
| Prime numbers | [StackOverflow: prime up to sqrt](https://stackoverflow.com/questions/54543956/finding-prime-number-using-the-square-root-method) |
| Official puzzle docs | [eightqueens — 01-edu public](http://public.01-edu.org/subjects/eightqueens/) |
| Eight queens theory | [Wikipedia: 8 queens](https://en.wikipedia.org/wiki/Eight_queens_puzzle) |
| Sample Go solutions | [01founders-crack/piscine-go](https://github.com/01founders-crack/piscine-go) |


***

### Task Recommendations

| Task | Skills/Methods | Tips |
| :-- | :-- | :-- |
| iterativefactorial | Standard loop, input checks | Return 0 for nb < 0, watch for overflow |
| recursivefactorial | Recursion, return for n==0 | Base case n < 0 or n == 0; no for loops |
| iterativepower | Iteration, check power < 0 | Return 1 if power == 0, 0 if <0 |
| recursivepower | Recursion, same checks | No for, base case power == 0 |
| fibonacci | Recursion, base cases \& -1 | Return -1 for index < 0, handle 0,1 at start |
| sqrt | Standard loop up to nb, square check | Return x if x\*x == nb; else 0 |
| isprime | Check divisors up to sqrt(nb) | Tip: use sqrt limit, start at 2 |
| findnextprime | Upward search, isprime each | Go up until finding a prime |
| eightqueens | Recursive backtracking | Ban row/col/diagonal conflicts |


***

### Best Practices

- Always implement both factorial and power problems using both iteration and recursion.
- Prime check optimization: Only test divisors to $\sqrt{n}$—all others are paired with smaller factors.
- Use a written isprime function for next-prime searches to avoid duplicating code.
- Backtracking for eight queens is easier with an array (index = row, value = column)—check for conflicts on each step.
- Test algorithms with edge and boundary inputs: 0, 1, invalid/very large numbers.

***

### Where to Find Example Solutions

- [01founders-crack/piscine-go](https://github.com/01founders-crack/piscine-go) — detailed solutions for all exercises in this block.
- [eightqueens — public subject 01-edu](http://public.01-edu.org/subjects/eightqueens/) — canonical description and pseudocode for “eight queens”.
- Video tutorials and articles on recursion and number sequences will speed learning for factorial and Fibonacci logic.

***


