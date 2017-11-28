# @media

ネストはメディアクエリでも使うことができます。<br>


```scss
.main {
    margln: 0 0 1em;
    section {
        width: 600px;
        @media screen and (max-width: 480px) {
          width: 400px;
        }
    }
}
```

CSSの場合はネストが使えないため、メディアクエリを書く位置が離れてしまって見通しが悪くなり、同じセレクタに指定したスタイルの関係性がつかみにくかったが、scssを使うと名前空間の中で記述できるので関係性がはっきりする。
