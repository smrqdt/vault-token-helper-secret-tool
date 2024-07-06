# vault-token-helper-secret-tool [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/smrqdt/vault-token-helper-secret-tool/main.svg)](https://results.pre-commit.ci/latest/github/smrqdt/vault-token-helper-secret-tool/main)

A [HashiCorp Vault](https://www.vaultproject.io/) [token
helper](https://www.vaultproject.io/docs/commands/token-helper) in a
few lines of POSIX shell code, using
[libsecret's](https://wiki.gnome.org/Projects/Libsecret)
`secret-tool`.

## Usage

Clone this repo or install the script somewhere some other way, run it
with the `enable` argument:

```shell
./vault-token-helper-secret-tool enable
```

### Multiple Vault clusters

Operates on the entry associated with the current `VAULT_ADDR` environment variable. If unset, a default token slot will be used.

## Alternatives, credits

Inspired by
[joemiller/vault-token-helper](https://github.com/joemiller/vault-token-helper),
but much smaller and simpler. For something more elaborate than this
one, as well as for support for other store backends besides what
libsecret works with, that'd be one alternative to look into.

Adapted from [scop/vault-token-helper-secret-tool](https://github.com/scop/vault-token-helper-secret-tool] to use `$VAULT_ADDR`.

## License

SPDX-License-Identifier: Apache-2.0
