# debug branches

Notes on how I can use branches to debug common issues:

create debug branch
    create branch cj-debug-<type-of-issue-here>
    commit debug changes

to debug master, rebase (pull master into mock branch, commit)

to debug a branch:
    git checkout <some-feature-branch>
    git checkout -b debugging-<some-feature-branch>
    git merge cj-debug-<type-of-issue-here>
    then if you discover a change to make, stash, switch back to <some-feature-branch>, unstash

