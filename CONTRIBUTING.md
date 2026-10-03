# Contributing

Found a mistake, or want to add something guix-related? Open a PR.

Please follow the style of previous commits (check `git log`).

## Entry format

Each entry is a link, a dash, and a short description that ends with a period:

```
- [some/guix-channel](https://example.com/some/guix-channel) - Packages for something useful.
```

The description starts with a capital letter and doesn't repeat the entry name. CI runs [awesome-lint](https://github.com/sindresorhus/awesome-lint) on every PR; run `npx awesome-lint` locally to check before pushing.

## Unmaintained entries

Entries with no updates for 3+ years, or archived, are marked with a trailing 💤, e.g.:

```
- [some/guix-config](https://example.com/some/guix-config) - Personal Guix configuration. 💤
```

The marker is a heads-up, not a removal - old configs in particular often stay useful as references. Entries that 404 or have moved should be removed instead.
