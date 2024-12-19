# Upgrading warnings to run-time errors

If you're seeing warnings for `RemovedIn20Warning` and want to make it a run-time error so that you can better catch them during testing, you can do:

```python
import warnings

from sqlalchemy.exc import RemovedIn20Warning

warnings.filterwarnings("error", category=RemovedIn20Warning)
```

I discovered this while working on [step 5](https://docs.sqlalchemy.org/en/20/changelog/migration_20.html#migration-to-2-0-step-five-use-the-future-flag-on-session) of migrating sqlalchemy from 1.4 to 2.0
