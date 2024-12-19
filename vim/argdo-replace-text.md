# argdo to replace text in arg list

open all files with a match: `vi \`rg -l before\``

then `:argdo %s/before/after/g`

save all with `:wa`

