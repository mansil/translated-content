---
title: KeyboardEvent.ctrlKey
slug: Web/API/KeyboardEvent/ctrlKey
---

{{APIRef("UI Events")}}

**`KeyboardEvent.ctrlKey`** は読み取り専用のプロパティで、このイベントが発生したときに <kbd>control</kbd> キーが押されていた (`true`) または押されていなかった (`false`) ことを表す論理値を返します。

## 値

論理値です。

## 例

```js
<html>
<head>
<title>ctrlKey の例</title>

<script type="text/javascript">

function showChar(e){
  alert(
    "Key Pressed: " + e.key + "\n"
    + "CTRL key pressed: " + e.ctrlKey + "\n"
  );
}

</script>
</head>

<body onkeypress="showChar(event);">
<p>CTRL キーを押したまま、または押さずに、任意の文字キーを押してください。<br />
また、 SHIFT キーと CTRL キーを同時に使用することもできます。</p>
</body>
</html>
```

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}

## 関連情報

- {{ domxref("KeyboardEvent") }}
