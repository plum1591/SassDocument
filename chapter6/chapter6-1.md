# 基本

```
css/
    - common.css
    - base.css
    - top.css
    - extend.css
    - utility.css
```
↑このようなスタイル用ディレクトリがあった場合、

```html
<link rel="stylesheet" type="text/css" href="css/common.css">
<link rel="stylesheet" type="text/css" href="css/base.css">
<link rel="stylesheet" type="text/css" href="css/top.css">
<link rel="stylesheet" type="text/css" href="css/extend.css">
<link rel="stylesheet" type="text/css" href="css/utility.css">
```
どんどんhtmlに増やして<head>要素を拡大するのは保守性が悪い。

```scss
// common.scss
@import 'scss/base';
@import 'scss/top';
@import 'scss/extend';
@import 'scss/utility';

```
↑ 上記のように記述するとhtmlで読み込むファイルは

```html
<link rel="stylesheet" type="text/css" href="css/common.css">
```
のみでおっけ！！！！
