# commitlint-casing-issue

Snake case and kebab case issues for scope and subject case

# Config used

```yml
rules:
  scope-case: [2, always, lower-case]
  subject-case: [2, always, lower-case]
```

# Checks

```bash
echo "feat(test): test" # Passes
echo "feat(TEST): test" # Fails
echo "feat(snake_case): test" # Passes (Expected: Fails)
echo "feat(kebab-case): test" # Passes (Expected: Fails)
```
