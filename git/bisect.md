```sh
# Start bisecting
git bisect start

# Indicate the bad commit
git bisect bad <bad_commit>

# Indicate the good commit
git bisect good <good_commit>

# Follow instructions to test each mid-point commit
# Mark each midpoint commit
git bisect good    # if the commit is good
git bisect bad     # if the commit is bad

# After finishing, exit bisect mode
git bisect reset
```
