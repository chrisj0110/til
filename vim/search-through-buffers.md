# search through buffers

To search through open buffers, first make sure arglist is populated with all open buffers:

```
:bufdo :args ## %
```

Then search through arglist:

```
:vimgrep /blah/ ##
```

From [SO](https://stackoverflow.com/a/30643432/59867).

