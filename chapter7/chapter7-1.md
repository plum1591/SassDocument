# 基本

@mixinでスタイルを定義して、@includeで呼び出します。<br>
初期値（$color: black）を設定しておくことも可能

```scss
@mixin box($color: black , $width , $height) {
  border: 1px dotted $color;
  width: $width;
  height: $height;
}

#menu {
  @include box(blue, 300px, 600px);
}
```
上記をコンパイルすると

```css
#menu {
    border: 1px dotted blue;
    width: 300px;
    height: 600px;
}

```
でコンパイルされる。
