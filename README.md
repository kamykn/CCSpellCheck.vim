# CCSpellCheck.vim
CCSpellCheck.vim is checking camelcase word spell.

## 1.Installation
### Installation with NeoBundle
```
NeoBundle 'kmszk/CCSpellCheck.vim'
```

## 2.Useage
### 2.i. Highlight bad spells.
You can add the following line to your vimrc files to highlight bad spells.

```
augroup CCSpellCheck
	autocmd!
	autocmd BufWinEnter,BufWritePost * call CCSpellCheck#check()
augroup END
```

### 2.ii. Correct bad spell.
Move the cursor over the wrong spelling and enter the following commands

```
Zc
```

### 2.iii. Add word as good spell list.
Add the selected word in visual mode with the following command.  
CCSpellcheck use 'spell' commands provided by vim as default.

FYI:
http://vim-jp.org/vimdoc-en/spell.html#zg

```
# Add selected word to spellfile
# => zg
Zg

# => zw
Zw

# => zug
Zug

# => zuw
Zuw

# Add selected word to the internal word list
# => zG
ZG

# => zW
ZW

# => zuG
ZUG

# => zuW
ZUW
```

