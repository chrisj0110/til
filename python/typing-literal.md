# typing.Literal

If you write a function that accepts a `str` but there are only certain valid values, then you have to trust callers to not send in a bad value (even a typo).

One option for better enforcement is to make it an `Enum` instead.

Or a more light-weight option is to use `typing.Literal`:

```python
from typing import Literal


def move(direction: Literal["n", "e", "s", "w"]) -> None:
    ...
```

This allows analysis to warn the caller if they're passing in an invalid value, and also allows LSP's to provide the user with auto-completion of valid values.

And if you need to define this in multiple places, you can do:

```python
from typing import Literal

Direction = Literal["n", "e", "s", "w"]


def move(direction: Direction) -> None:
    ...

def go_back(direction: Direction) -> None:
    ...
```

