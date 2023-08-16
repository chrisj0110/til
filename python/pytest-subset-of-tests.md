# Run subset of tests in pytest

You can mark a test function:

```python
@pytest.mark.regression()
def test_important_regression_scenario()
    ...

@pytest.mark.regression()
def test_important_regression_scenario_2()
    ...

def test_trivial_one_off_scenario()
    ...
```

Then you can run the 2 `regression` tests with -m:

```bash
pytest -m 'regression' test_suite.py
```

To test everything in the file except the regression cases:

```bash
pytest -m 'not regression' test_suite.py
```
