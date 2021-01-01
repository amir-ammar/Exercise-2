###### Exercise-2
### fzf 
  ## Definition
  `fzf` itis interactive finder dialogue and instant feedback that filters items as you type . the primary use case for fzf is to search for files on the command line.
  `fzf` supports fuzzy matching so you can just type several characters in a row and it will match lines with those characters scattered across the string.
  
  
  ## installion :(*just type this command line*)
  `sudo apt install fzf`
  
  
  ## matching :
    `fzf` support 2 types of matching :
      1- exact matching
      2- fuzzy matching
   # example searching for a file :
   ```
   fzf
   "item you search for"
   ```
   # what if you don't like fuzzy matching ??!
     just type single quote before the item you search for.
    
   > if you do not want fuzzy matching .
   ```
   fzf
   ' "item you search for"
   ```
   > another way to do it
   ```
   fzf -e
   ```
   # ~~it does not support globe button~~ as :
   ```
   fzf
   *.txt
   ```
   
   
  ## results of the search :
   you can select some items of the results of the search with the `tab` key . it seems not useful unless you redirect your output to another file with `|` (pipe).
   
   
   # also you can combine it with `history` command to search for your recent commands :
   ```
   history | fzf "item you search for"
   ```
   # if you memorise just a little of your file name . no need to go to your file manager and find it . you can use `fzf` to search for it as it fuzzy completion can be triggered by dedicated sequence :
   
   > **(double star) - trigger fuzzy completion
   
   ```
   vim ~/.compile.txt/**
   ```
   
   
  ## for further explaination just visit >> [fzf tutorials](https://www.freecodecamp.org/news/fzf-a-command-line-fuzzy-finder-missing-demo-a7de312403ff/)
  
  
###   
  
  
  
  
  
  
  
