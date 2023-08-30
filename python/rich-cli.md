# rich-cli package

[rich-cli](https://github.com/textualize/rich-cli) enhances terminal output. For example:

```bash
$ echo '{"test":  "testing", "test2": [{"this": "is in a list!"}]}' | rich - --json
{
  "test": "testing",
  "test2": [
    {
      "this": "is in a list!"
    }
  ]
}
```