# FortranDictionary_vim
A FORTRAN keyword dictionary, or word list, made to use specially with vim's built-in dictionary completion.

## HOW TO USE:
#### 1. Add this file to your .vim directory

#### 2. Into your .vimrc add a FORTRAN type file: (or you can use your own config)
```
au Bufred, BuFNewFile *f, *f90, *f95 set filetype=fortran
```

#### 3. add the file as a dictionary completion option
```
au FileType fortran set dictionary+=/path/to/.vim/dict/fortran
```
