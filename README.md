# JavaScriptドキュメント
![](https://img.shields.io/github/last-commit/kelp-of-truth/JS-Document) ![](https://img.shields.io/github/forks/kelp-of-truth/JS-Document?style=social) ![](https://img.shields.io/github/stars/kelp-of-truth/JS-Document?&style=social)

[目次]
- [Hello world!](./hello-world/README.md)
- [計算式](./math/README.md)
- [文字と変数の混ざった値の出力](./extra1/README.md)
- [条件分岐]()
- [反復処理]()
---

JavaScriptオンラインエディタ(Node.js)<br>

[Replit](https://replit.com/languages/nodejs)


## Replitで入力値を取得する方法
Replitでコンソールの入力値を取得するには`prompt()`関数を使います。<br/><br/>
***入力***
```js
// 入力値を変数 input に代入
var input = prompt("");
// 変数 input をコンソールに出力
console.log(input);
```
***出力***
```
> 
```
<br>

また、`prompt("メーッセージ")`のように書く事もできます。日本語を入れると表示がバグります。<br/><br/>
***入力***
```js
prompt("Hello");
```
***出力***
```
Hello> 
```
