# Using Annotated in typer

As of version 0.9.0 `typer` recommends using `Annotated`. Docs start [here](https://typer.tiangolo.com/tutorial/arguments/optional/).

An example:

```python
import typer
from typing_extensions import Annotated

def main(
    last_name: Annotated[str, typer.Argument(help="Last name")],
    first_name: Annotated[str, typer.Argument(help="First name")] = "Joe",
    verbose: Annotated[bool, typer.Option("--verbose", "-v", help="Verbose mode")] = False,
) -> None:
    ...
```

`--help` gives:

```
 Usage: script.py [OPTIONS] LAST_NAME [FIRST_NAME]

┌─ Arguments ────────────────────────────────────────────────────────────────┐
│ *    last_name       TEXT          Last name [default: None] [required]    │
│      first_name      [FIRST_NAME]  First name [default: Joe]               │
└────────────────────────────────────────────────────────────────────────────┘
┌─ Options ──────────────────────────────────────────────────────────────────┐
│ --verbose  -v        Verbose mode                                          │
│ --help               Show this message and exit.                           │
└────────────────────────────────────────────────────────────────────────────┘
```
