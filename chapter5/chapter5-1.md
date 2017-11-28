# 基本

```scss
@function Double($value) {
  @return round($value * 2);
}

.box{
  width: Double(300px);
}
```
