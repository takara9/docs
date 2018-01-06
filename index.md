# Markdownで作成したウェブページのサンプル

GitHubを利用して、情報を共有するプロジェクトが増えています。 例としてKubernetes プロジェクトの文書や IBM Cloud のマニュアルページも GitHubを使って作成されています。 GitHubを利用することでプロジェクトの沢山のメンバーが同時に作業できて、課題の共有や修正依頼を挙げるなど、文書作成のプロジェクトを円滑に進めていく事ができます。

僕はGitHubの人じゃないですが、この記事で紹介する GitHub pages は、HTMLを覚えなくても簡単なマークダウンで作成できて、テーマを設定によって、見やすい書式へ自動変換される優れたものです。 


### レイアウト設定

マークダウンの先頭に、次のコマンドをセットすることで、レイアウトを設定できます。このレイアウトの設定ファイル`default`は `_layouts/default.html` に配置されます。　この設定によって画面のデザインを変更する事ができます。

~~~
---
layout: default
---
~~~


### テキストの文字種

テキストは、**ボールド**、_イタリック_、~~取り消し~~、そして `keyword` を利用できます。



### 他文書へのリンク

* [同一ディレクトリ内のページへのリンク](another-page)
* [外部サイトへのリンク](http://www.ibm.com/)



### ホワイト・スペース 

パラグラフ（段落）の間には、ホワイト・スペースを入れる必要があります。マークダウンにホワイトスペースを入れることで、`<p>`が埋め込まれ、HTMLのパラグラフとしてタグが設定されます。 ここでのホワイト・スペースは空白行のことを指しています。


#### ホワイト・スペースが無いケース

この頃は書道がひどく流行して来て、世の中に悪筆が横行している。なまじっか習った能筆風な無性格の書や、擬態の書や、逆にわざわざ稚拙をたくんだ、ずるいとぼけた書などが随分目につく。
絶えて久しい知人からなつかしい手紙をもらったところが、以前知っていたその人の字とは思えないほど古法帖めいた書体に改まっている、うまいけれどもつまらない手紙の字なのに驚くような事も時々ある。しかしこれはその人としての過程の時期であって、やがてはその習字臭を超脱した自己の字にまで抜け出る事だろうと考えてみずから慰めるのが常である。やはり書は習うに越した事はなく、もともと書というものが人工に起原を発し、伝統の重畳性にその美の大半をかけているものなので、生れたままの自然発生的の書にはどうしても深さが無く、その存在が脆弱《ぜいじゃく》で、甚だ味気ないものである。


#### ホワイト・スペースを入れたケース

この頃は書道がひどく流行して来て、世の中に悪筆が横行している。なまじっか習った能筆風な無性格の書や、擬態の書や、逆にわざわざ稚拙をたくんだ、ずるいとぼけた書などが随分目につく。

絶えて久しい知人からなつかしい手紙をもらったところが、以前知っていたその人の字とは思えないほど古法帖めいた書体に改まっている、うまいけれどもつまらない手紙の字なのに驚くような事も時々ある。しかしこれはその人としての過程の時期であって、やがてはその習字臭を超脱した自己の字にまで抜け出る事だろうと考えてみずから慰めるのが常である。やはり書は習うに越した事はなく、もともと書というものが人工に起原を発し、伝統の重畳性にその美の大半をかけているものなので、生れたままの自然発生的の書にはどうしても深さが無く、その存在が脆弱《ぜいじゃく》で、甚だ味気ないものである。


### ヘッダー

次のサンプルコードの様に、ヘッダにタグをつけて、ジャンプ先としてリンクもできます。

~~~
# [](#header-1)Header 1
~~~

# [](#header-1)ヘッダー 1

これはヘッダーの後に続く普通のパラグラフです。 GitHubは、バージョン・コントロールと共同作業のためのコード・ホスティング・プラットフォームです。 これによって、様々な場所のあなたや他の人が共同で働くプロジェクトができます。

## [](#header-2)ヘッダー 2

> これはヘッダーに続く引用パラグラフを表現するブロッククオートです。
>
> とても重要なこと、または、好まない変なことの引用として利用します。



### [](#header-3)ヘッダー 3

##### JavaScriptのコード

'`'を３個続けることで、コードを表記するエリアになります。 この３個の連続の後にプログラム言語の略称を書くことで、適切な色分けができます。

~~~
```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```
~~~

上記を適用した実施例

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

##### Rubyのコード

同様にRubyのケース

~~~
```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```
~~~

上記の表記を適用した実施例

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```



#### [](#header-4)ヘッダー 4

*   ヘッダーに続く番号なし箇条書き
*   ヘッダーに続く番号なし箇条書き
*   ヘッダーに続く番号なし箇条書き



##### [](#header-5)ヘッダー 5

1.  番号付きリスト
2.  番号付きリスト
3.  番号付きリスト



###### [](#header-6)ヘッダー 6

テーブル（表）形式の記述です。

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |


### 水平線

次の方法で、水平線を描画できます。

* * *

~~~
* * *
~~~



### 番号付きリスト

リストの各行先頭に`1.`とするだけで、番号は自動的に付与します。

1.  Item one
1.  Item two
1.  Item three
1.  Item four


### ネストしたリスト

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### イメージの挿入

```
![](https://assets-cdn.github.com/images/icons/emoji/octocat.png)
![](https://guides.github.com/activities/hello-world/branching.png)
```

![](https://assets-cdn.github.com/images/icons/emoji/octocat.png)
![](https://guides.github.com/activities/hello-world/branching.png)



### HTML形式の定義リスト

```HTML
<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>
```

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>




### 長いパラグラフを１行で表示

この様な長い文を１行で表示したいときは```で上下を囲む

Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.



```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```


### END OF FILE


