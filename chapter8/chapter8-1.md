# 基本

@extendを使用することでセレクタのスタイルを継承することができし、
継承したうえでスタイルの追加や上書きも行うことができる。

```scss
.btn{
  padding: 10px 20px;
  border: 2px solid blue;
  border-radius: 3px;
  background-color: lightgray;
}

.btn-submit{
  @extend .btn; //.btnのスタイルを継承
  background-color: lightblue; //スタイルの上書き
  font-size: 1.5em; //スタイルの追加
}
```
上記をコンパイルすると

```css
.btn, .btn-submit {
  padding: 10px 20px;
  border: 2px solid blue;
  border-radius: 3px;
  background-color: lightgray;
}

.btn-submit {
  background-color: lightblue;
  font-size: 1.5em;
}

```
でコンパイルされる。
