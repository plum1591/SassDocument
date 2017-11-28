# SASSとSCSS

最初に作られてのが**SASS**記法。


### SASS
・セレクタの後の{～}(波括弧)の代わりにインデント<br>
・値の後の；（セミコロン）は省略<br>
・CSSと互換性がなく、CSSの書式で書くとエラーになってしまう<br>
<br>
```sass
ul
  margln: 0 0 1em
  li
    margln-bottom: 5px
```
<br>
### SCSS
・｢SassyCSS｣の略で､翻訳すると「カッコいいCSS｣や「イカしたCSS」という意味<br>
・CSSとの互換性を高く、CSSの書式で書いてもエラーにならない<br>
・現在、Sassを指す場合はSCSS記法が一般的で、公式サイトでもSCSS記法がデフォルトで表示されている。
<br>
```scss
ul {
  margln: 0 0 1em;
  li {
    margln-bottom: 5px;
  }
}
```
