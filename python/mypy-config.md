# Mypy configuration

Some `mypy.ini` settings I like to use:

```ini
[mypy]

# uses sqlalchemy[mypy]
plugins = sqlalchemy.ext.mypy.plugin

# these are to handle naming conflicts (two dirs with the same name in diff packages): https://mypy.readthedocs.io/en/stable/running_mypy.html#mapping-file-paths-to-modules
namespace_packages = True
explicit_package_bases = True

# if third-party package doesn't have stubs, just treat everything as Any. (It would be better to find/make stubs)
ignore_missing_imports = True

# error whenever it encounters a function definition without type annotations
disallow_untyped_defs = True

# error whenever it encounters a partly annotated function definition
disallow_incomplete_defs = True

# x: int = None param must be x: Optional[int] = None
no_implicit_optional = True

# warns about casting an expression to its inferred type.
warn_redundant_casts = True

# warns when you return Any
warn_return_any = True

# prohibit comparisons of non-overlapping types, and similar identity and container checks.
strict_equality = True

# output
pretty = True
```

Can also configure these in VSCode settings:

```json
"python.linting.mypyEnabled": true,
"python.linting.mypyArgs": [
    "--no-namespace-packages",
    "--explicit-package-bases",
    "--ignore-missing-imports",
    "--disallow-untyped-defs",
    "--disallow-incomplete-defs",
    "--no-implicit-optional",
    "--warn-redundant-casts",
    "--warn-return-any",
    "--strict-equality",
    // "--config-file=mypy.ini",  doesn't seem to work yet: https://github.com/microsoft/vscode-python/issues/6678
],
```
