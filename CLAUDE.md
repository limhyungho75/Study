# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository overview

This is a personal study/scratch repository with almost no content yet:

- `Readme.md` — a one-line description in Korean ("이것은 테스트입니다." / "This is a test.").
- `Test.py` — a single Python script containing only `print 'aaaa'`.

There is no build system, package manifest, dependency list, linter config, or test suite.

## Running code

`Test.py` uses **Python 2** print-statement syntax, so it fails under Python 3 with a `SyntaxError`:

```sh
python2 Test.py   # works if Python 2 is installed
python3 Test.py   # SyntaxError
```

If you modify or add Python files, ask the user whether to keep Python 2 syntax or migrate to Python 3 (e.g. `print('aaaa')`) rather than changing it silently.
