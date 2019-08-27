# sjpCLVi
Polish Dictionary based on sjp.pl - Command Line Interface and Vim (nvim) implementation

## Usage:
```
./sjpcli <word>

example:
d3s ~$ ./sjpcli żołądź
zoladz
dopuszczalne w grach 

(r. meski)
1. owoc debu; zoladz (r. zenski)
2. kolor w kartach, trefl; zoladz (r. zenski)
```

## Implementation with vim:
 - Make sure that `sjpcli` is executable (`chmod +x sjpcli`)
 - Make sure you know its directory
 - Modify `.vimrc` or `init.vim`, adding this line:
   - `vmap <F9> y:execute '!/<DIRECTORY_OF_SJPCLI>/sjpcli ' . escape(getreg('0'), '/')<CR>`
 - Modify `<DIRECTORY_OF_SJPCLI>` to your known directory
 
## Usage in vim:
> this can be modified in your vim config
 - Select word using `Visual mode`
 - Press F9 key
