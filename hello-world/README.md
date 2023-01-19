# Hello world!

## こんにちは、世界！
　「こんにちは、世界！」プログラムでは、初めにHello world!から始めます。<br>
　JavaScript[^1]ではコンソールに文字を出力するには`console.log()`関数を使います。カッコの中にダブルクオーテーション（"←これ）で囲みます。はじめにコンソールに「Hello world!」と出力してみましょう。

***入力***
```js
console.log("Hello world!");
```
***出力***
```
Hello world!
```

## 変数の宣言
　変数というのは、値を保存しておくようなものです。変数を作るには、`var 変数名 = 値;`のように書きます[^2]。では、変数に保存した値をコンソールに出力してみましょう。
 
***入力***
```js
// 「hello」という変数を作り、変数helloに「Hello world!」を代入
var hello = "Hello world!";
// コンソールに変数helloを出力
console.log(hello);
```
***出力***
```
Hello world!
```
ここで気をつけることは、変数を出力する場合は、ダブルクオーテーションで囲まないということです[^3]。試しにダブルクオーテーションで囲んで実行しましょう。

***入力***
```js
var hello = "Hello world!";
console.log("hello");
```
***出力***
```
hello
```
このように「hello」という文字が出力されてしまいます。

## 代入値なしでの変数宣言
　変数の宣言時には初期値を設定せず、変数を作るだけという事もできます。

***入力***
```js
var hello;
console.log(hello);
```
***出力***
```
undefined
```
このときの値を出力してみると、`undefined`が返ってきます。`undefined`というのは、「未定義」という意味です。`undefined`ではなくなにも文字を返さないということをしたい場合は、変数に`""`という値を代入します。

***入力***
```js
var hello="";
console.log(hello);
```
***出力***
```

```

## 変数の値の変更
　`var`で宣言した変数は値の変更（再代入）ができます。再代入する際は最初に`var`をつけずに、`変数名 = 値;`のようにして再代入します。
 
***入力***
```js
// 変数を宣言
var hello="Hello world!";
// 値を再代入
hello="こんにちは、世界！";
// 出力
console.log(hello);
```
***出力***
```
こんにちは、世界！
```

## const
`const`は`var`と同じように変数を宣言ができますが、`const`は`var`と違って値の再代入ができません（つまり読み取り専用ということです）。

***入力***
```js
const hello="Hello world!";
console.log(hello);
```
***出力***
```
Hello world!
```
`const`を使うときの注意は、宣言時になんでもいいので必ず値を代入するということです。値を代入せずに宣言してみましょう。
 
***入力***
```js
const hello;
console.log(hello);
```
***出力***
 ```
 SyntaxError: Missing initializer in const declaration
 ```
 SyntaxError（シンタックスエラー）[^4]というのが出てしまいます。エラーの内容は「constの初期値が定義されていません。」というようなものです。
<br><br>



[<前のページ](https://github.com/kelp-of-truth/JS-Document) \[[1](./)\] [次のページ>](../math)


[^1]: 本当はNode.jsですが、ここではJavaScriptと呼びます。
[^2]: 変数を宣言する方法は他にもあり、`let`、`const`があります。`let`は、変数の再宣言ができません。（`var`はできる）`const`は再代入も再宣言もできません。
[^3]: 数字も文字として「1」を使用する場合はダブルクオーテーションで囲みますが、数字として「1」を使用する場合は囲みません。
[^4]: Syntaxというのは「構文」という意味で、つまり構文エラーということです。
