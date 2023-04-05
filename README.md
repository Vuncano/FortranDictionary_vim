# FortranDictionary_vim
A FORTRAN keyword dictionary, or word list, made to use specially with vim's built-in dictionary completion.

## HOW TO USE:
#### 1. Add this file to your .vim directory

#### 2. Into your .vimrc add a FORTRAN type file: (or you can use your own config)
```
au Bufred, BuFNewFile *f, *f90, *f95 set filetype=fortran
```
This sets a filetype called "fortran" for files that end with `.f`, `.f90`, `.f95`

#### 3. add the file as a dictionary completion option
```
au FileType fortran set dictionary+=/path/to/.vim/dict/fortran
```
`set dictionary+=/path/to/.vim/dict/fortran` tells vim to use the file you're pointing as a dictionary.
`au FileType fortran` tells vim to only set said config when you're working with fortran file type, hence the dictionary completion will not work when using other file types.

## HOW TO UNSET THE DICTIONARY
Vim's `:help  dictionary` recommends you to not just comment the line or delete it, nor to just delete the file, but insted to use
```
dictionary-=/path/to/dictionary
```
