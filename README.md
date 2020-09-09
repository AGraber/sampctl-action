# sampctl-action
This action sets up sampctl in the environment for use in actions.

This doesn't work on Windows (no reason to use Windows anyways, output is the same).

# Usage
Basic example:

```yml
steps:
  - uses: actions/checkout@v2
  - uses: AGraber/sampctl-action@v1
      with:
      version: '1.9.1' # optional, 1.9.1 by default
  - run: sampctl p build --forceEnsure
```
