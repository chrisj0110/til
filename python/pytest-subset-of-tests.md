# Run subset of tests in pytest

For all of the following, you can first output what it plans to run without running tests, using `--setup-plan`

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

You can use `-k` to select function(s) and class(es):

```bash
pytest -k 'test_function1 or test_function2' test_suite.py
```

```bash
pytest -k 'test_function1 and ClassName1' test_suite.py
```

