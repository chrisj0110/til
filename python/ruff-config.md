# Ruff config

Here are some ruff rules I've used. Teams should agree on what to use and what not to use.

```toml
extend-select = [
    "W",  # pycodestyle warnings
    "I",  # isort
    "UP006",  # pyupgrade: use builtin for type annotations
    "B",  # flake8-bugbear
    "A",  # flake8-builtins
    "C40",  # flake8-comprehensions
    "ISC",  # flake8-implicit-str-concat
    "ICN",  # flake8-import-conventions
    "INP",  # flake8-no-pep420
    "PIE",  # flake8-pie
    "PT",  # flake8-pytest-style
    "RSE",  # flake8-raise
    "RET",  # flake8-return
    "RUF100",  # finds unnecessary 'noqa' directives
    "SIM",  # flake8-simplify
    "TID",  # flake8-tidy-imports
    "PTH",  # flake8-use-pathlib
]

ignore = [
    "E501",  # ignore "line too long", let black handle it
    "F841",  # don't wipe out unused vars, it might surprise devs
    "SIM102",  # auto-combining if statements can make them harder to read
    "SIM108",  # let devs decide to not use ternary expressions
    "SIM118",  # not always safe to use this one - it caused an issue with sqlalchemy
    "SIM211",  # auto-fixing these boolean expressions might make them harder to read
    "SIM300",  # Yoda conditions are fine when using sqlalchemy
]

line-length = 160

target-version = "py39"
```

All rules are at https://beta.ruff.rs/docs/rules/
