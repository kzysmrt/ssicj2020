# テキストフィールドとJavaScriptの連携
本章では，テキストフィールドへの入出力を学びます．

## テキストフィールドを作る

htmlを使ってテキストフィールドを作るには，inputタグを使います．
```
<input type="text">
```

### hint
右側のオレンジの部分にテキストフィールドを作るためのタグを入力してみましょう．

### main(index.html)

<div code src='2-1'></div>

## テキストフィールドの初期値作る

テキストフィールドの初期値を指定するには，value属性を使います．
```
<input type="text" value="2">
```

### main(index.html)

<div code src='2-2'></div>

## テキストフィールドから値を取得する

テキストフィールドに記入された文字を取得するには，
```
var x = document.getElementById('[id名]').value;
```
プログラムを使います．
```
document.getElementById('[id名]')
```
でbodyタグの中身から，[id名]のついた要素（タグ）を探し，そのタグの属性であるvalueを
```
.value
```
で取得し，変数xに格納します．

### main(index.html)

<div code src='2-3'></div>

## テキストフィールドに値を入力する

テキストフィールドに値を入力するには，
```
documnet.getElementById('[id名]').value = x;
```
(xは定義済みの変数)プログラムを使います．

### main(index.html)

<div code src='2-4'></div>

## テキストフィールドから取得した文字列を数字に変換し，計算を行う

テキストフィールドから入力された値は，文字列になっています．したがって，入力された値を利用して計算をするには，数字の変数に変換する必要があります．

文字列を数字に変換するには，
```
x = Number(x);
```
(xは定義済みの変数)プログラムを使います．

Number関数で，文字列を数字に変えることができます．
さあ，足し算プログラムを作ってみましょう．

### main(index.html)

<div code src='2-5'></div>


