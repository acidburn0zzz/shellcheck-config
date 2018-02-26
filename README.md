**Problem** : as of v0.4.7 ShellCheck [does not support](https://github.com/koalaman/shellcheck/wiki/Ignore) configuration files.

**Proposed solution** : use same config format from related [Hadolint](https://github.com/hadolint/hadolint) tool which itself uses ShellCheck.

Sample configuration for `.shellcheck.yaml`: 

```sh
ignored:
  - SC2140
  - SC2086
  - SC2046
```

This configuration is supported by [CodeFactor](https://www.codefactor.io).
