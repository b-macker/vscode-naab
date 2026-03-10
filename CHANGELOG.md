# Changelog

## [0.2.0] - 2026-03-10

### Added
- 8 missing operators: `->`, `::`, `..=`, `%=`, `?`, `:`, `|`, `&`
- Polyglot `-> TYPE` return syntax highlighting (JSON Sovereign Pipe)
- `BLOCK-LANG-N` identifier highlighting
- Punctuation highlighting for `:`, `?`, `;`
- 22 code snippets (main, fn, for, polyglot blocks, govern.json, etc.)
- Gallery banner and homepage in package.json

### Fixed
- Removed `var` from keyword declarations (not a NAAb keyword)
- Removed `<<`/`>>` from bracket pairs (polyglot blocks are not bracket pairs)
- Added `module`, `catch`, `else` to folding markers
- Range operator now matches both `..` and `..=`

## [0.1.0] - 2026-03-10

### Added
- Initial release
- Syntax highlighting for all 41 NAAb keywords
- Polyglot block highlighting for 13 languages
- String interpolation support (`${expr}`)
- Standard library module recognition (14 modules)
- Comment support (`//`, `#`, `/* */`)
- Bracket matching and auto-closing
- Code folding
