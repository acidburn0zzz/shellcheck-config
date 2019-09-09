**problème**: pour la version 0.4.7 ShellCheck [ne doit pas supporter](https://github.com/acidburn0zzz/shellcheck/wiki/Ignore) configuration files.

**Solution proposer**: utiliser la même configuration de format relative à l'outil [Hadolint](https://github.com/hadolint/hadolint) qui lui même utilise ShellCheck.

Exemple de configuration pour `.shellcheck.yaml`: 

```sh
ignored:
  - SC2140
  - SC2086
  - SC2046
```

Cette configuration est supportée par [CodeFactor](https://www.codefactor.io).
