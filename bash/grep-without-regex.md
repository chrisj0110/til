# Grep without regex

If you are trying to grep for something with characters like `.` or `+` in it, you might get unexpected results if you forget that grep uses regex.

To search for a fixed string instead, you can use `grep -F`.
