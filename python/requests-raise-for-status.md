# Requests response.raise_for_status()

The `requests` package can raise an HTTPError exception if there is an HTTP error:

```python
response = requests.get(url)
response.raise_for_status()
```
