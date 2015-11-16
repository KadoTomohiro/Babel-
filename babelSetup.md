# babel setupメモ

`process.argv`:
node実行時のコマンドライン引数を含む配列

インデックス|	内容
:---------|:----------
0         |node（固定値）
1         |JSファイルのパス
2以降      |コマンドライン引数の内容

~~~ js
// コマンドライン引数の配列のみ取得
process.argv.splice(2);
~~~

`` `Hello ${arg}` ``: [Template strings](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/template_strings)

* バッククォート(`` ` ``)で囲む
* プレースホルダー`${expression}`を含めることで動的な文字列生成を読みやすく記述できる

~~~ js
"Fifteen is " + (a + b) + " and　not " + (2 * a + b) + "."
~~~

~~~ js
`Fifteen is ${a + b} and\nnot ${2 * a + b}.`
~~~
