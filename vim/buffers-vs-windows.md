# buffers vs windows

In vim you can open file `a.txt`, then `:split b.txt`, giving you two windows. You can then close the `b.txt` window.

You now have one window with `a.txt`, but you still have both buffers, which you can see using `:ls`.

You can navigate between the two buffers using `:bnext` and `:bprev`.

You can close a buffer using `:bd`

