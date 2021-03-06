# hnix

Haskell parser, evaluator and type checker for the Nix language.

## Prerequisites

Nix is installed and in your `$PATH`.

## Getting Started

```bash
$ git clone https://github.com/jwiegley/hnix.git
...
$ cd hnix
$ cabal2nix --shell . > default.nix
$ nix-shell
...
$ cabal test
...
$ cabal bench
...
$ ./dist/build/hnix/hnix --help
```

## How you can help

If you're looking for a way to help out, try taking a look [here](https://github.com/jwiegley/hnix/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22+no%3Aassignee).  When you find an issue that looks interesting to you, comment on the ticket to let others know you're working on it; look for others who might have done the same.  You can talk with everyone live on [gitter](https://gitter.im/haskell-nix/Lobby).

When you're ready to submit a pull request, test it with:
```
nix-shell --run "LANGUAGE_TESTS=yes cabal test"
```

Make sure that all the tests that were passing prior to your PR are still passing afterwards; it's OK if no new tests are passing.
