# NAAb Language for VS Code

Syntax highlighting and language support for the [NAAb programming language](https://github.com/b-macker/NAAb) — the first programming language with built-in AI governance.

## Features

- Syntax highlighting for `.naab` files
- Polyglot block highlighting (`<<python ... >>`, `<<rust ... >>`, etc.)
- Variable binding highlighting (`<<python[x, y] ... >>`)
- String interpolation (`"${expr}"`)
- Standard library module recognition
- Comment support (`//`, `#`, `/* ... */`)
- Bracket matching and auto-closing
- Code folding

## What is NAAb?

NAAb is a polyglot programming language that integrates 12 languages (Python, JavaScript, Rust, C++, Go, and more) with a built-in governance engine. A single `govern.json` file enforces code quality, security, and correctness across all languages — catching hallucinated APIs, oversimplified stubs, and security issues before code executes.

```naab
main {
    let numbers = [10, 20, 30, 40, 50]

    // Python for statistics
    let stats = <<python[numbers]
import statistics
f"mean={statistics.mean(numbers)}"
>>

    // Rust for performance
    let hash = <<rust
fn main() {
    println!("{:x}", md5::compute("hello"));
}
>>

    print(stats)
    print(hash)
}
```

## Links

- [NAAb Language](https://github.com/b-macker/NAAb)
- [NAAb Website](https://b-macker.github.io/NAAb/)
- [Governance Builder](https://b-macker.github.io/NAAb/governance.html)
- [TextMate Grammar](https://github.com/b-macker/naab-grammar)

## License

MIT
