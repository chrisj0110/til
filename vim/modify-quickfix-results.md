# modify quickfix results

if you have results in the quickfix list and want to delete all those lines, you can do `:cdo normal dd | w`

To modify text, `:cdo s/varname/new_varname/gc` - the last `c` is so that it will ask you to confirm for each one. Then `:wa` to save all buffers. via [youtube](https://www.youtube.com/watch?v=wOdL2T4hANk)

Can also modify and save all buffers directly like `:cdo s/varname/new_varname/g | w`

