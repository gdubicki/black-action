# *** ARCHIVED ***

I suggest using the [official GitHub action for Black](https://black.readthedocs.io/en/stable/integrations/github_actions.html) instead.

# *** ARCHIVED ***

# Black Code Formatter GitHub Action

A GitHub action that runs [black code formatter](https://github.com/ambv/black) for Python.

## Example Workflow

```workflow
workflow "Example Workflow" {
  on = "push"
  resolves = ["Lint"]
}

action "Lint" {
  uses = "lgeiger/black-action@master"
  args = ". --check"
}
```

For a full list of possible `args` checkout the [black docs](https://github.com/ambv/black#command-line-options).
