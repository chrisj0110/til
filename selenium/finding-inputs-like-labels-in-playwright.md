# finding inputs like labels in playwright

In playwright you can find an input by label: [https://playwright.dev/python/docs/locators#locate-by-label](https://playwright.dev/python/docs/locators#locate-by-label)

You can mimic this behavior using xpaths in selenium:

```python
input_element = driver.find_element(By.XPATH, "//label[text()='Property Name']/parent::div//input[1]")
```

First, it gets the label with text "Property Name": `//label[text()='Property Name']`

Second, it gets the parent div of that label element: `/parent::div`

Third, it gets the first input within that parent div: `//input[1]`

Note: this might work too using `following-sibling` (untested):

```python
input_element = driver.find_element(By.XPATH, "//label[text()='Property Name']/following-sibling::input")
```

