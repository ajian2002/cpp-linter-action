Github action for linting the C code.
Uses clang-tidy, clang-format, and cppcheck.

Example of usage:
```
name: c-linter

on: [pull_request]
jobs:
  c-linter:
    name: c-linter
    runs-on: ubuntu-latest
    steps:
      - name: c-linter
        uses: ajian2002/cpp-linter-action@master
    env:
        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
