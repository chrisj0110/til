# beautifulsoup

To get the first link whose text starts with "Click here for":

```python
link = next(l for l in soup.find_all("a") if l.text and l.text.startswith("Click here for"))
```

Documentation is [here](https://beautiful-soup-4.readthedocs.io/en/latest/)

