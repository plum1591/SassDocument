# 基本

こんなHTMLがあるとして、
```html
<main class="main">
    <section>
        <h1>SASS</h1>
        <p>sassのネストについて</p>
        <p class="notes">※深すぎないように</p>
    </section>
</main>
```

こんなスタイルをつけたいなーって場合に、
```css
main {
  margln: 0 0 1em;
}

main section {
  margln-bottom: 5px;
}

main section h1 {
  font-size: 14px;
}

main section p {
  font-size: 10px;
}

main section p.notes {
  color: red;
}
```

<br>
これじゃ、なんどもmainとsectionを記述しないとならないし、周りのスタイルの関係がわかりづらい。ので、

```scss
main {
    margln: 0 0 1em;

    section {
        margln-bottom: 5px;

        h1 {
            font-size: 14px;
        }

        p {
            font-size: 10px;

            &.notes {
                color: red;
            }
        }
    }
}
```

↑このように記述すると、全体の関係生がわかりやすくなる。
