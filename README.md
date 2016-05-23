Ios Fixed

====

iosでよくある `header -> input`の入れ子で`focus`した時に上下どっちかにスクロールするバグを修正する。

`focus`した際に、位置を取得して、それを`body`に`position: fixed; top:{位置};`を追加している。なので、`focus`中、または`click`後は、`blur`にならないと解除されないことに注意。

## How to use

```javascript
$(function() {
	$('input[type="text"]').IoxFixed();
});
```

## 修正したいこと

* ios以外ではfixedする必要はないので、どうしようか考え中
* 本README.mdを英語化
