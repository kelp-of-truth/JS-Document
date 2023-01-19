# JavaScriptドキュメント
![](https://img.shields.io/github/last-commit/kelp-of-truth/JS-Document) ![](https://img.shields.io/github/forks/kelp-of-truth/JS-Document?style=social) ![](https://img.shields.io/github/stars/kelp-of-truth/JS-Document?&style=social)

[目次]
- [Hello world!](https://github.com/kelp-of-truth/JS-Document/tree/main/hello-world)
- [計算式]()
- [条件分岐]()
- [反復処理]()
---

**JavaScriptオンラインエディタ(Node.js)**<br/>
[Replit](https://replit.com/languages/nodejs)<br>
---
## Replitで入力値を取得する方法
Replitでコンソールの入力値を取得するには`prompt()`関数を使います。
```js
// 入力値を変数 input に代入
var input = prompt("");
// 変数 input をコンソールに出力
console.log(input);
```
また、`prompt("メーッセージ")`のように書く事もできます。日本語を入れると表示がバグります。<br/><br/>
***入力***
```js
prompt("Hello");
```
***出力***
```
Hello> 
```
