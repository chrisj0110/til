# past commit messages

To search for text in commit messages since a date:

```bash
git log --since="2024-03-19" --grep "some text"
```

Or relative:

```bash
git log --since="3 weeks ago" --grep "some text"
```

Can also look for date ranges:

```bash
git log --after="2024-03-19" --until="2024-03-20" --grep "some text"
```

