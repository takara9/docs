# マークダウンで作成したウェブページのサンプル

GitHubを利用して、情報を共有するプロジェクトが増えています。 例としてKubernetes プロジェクトの文書や IBM Cloud のマニュアルページも GitHubを使って作成されています。 GitHubを利用することでプロジェクトの沢山のメンバーが同時に作業できて、課題の共有や修正依頼を挙げるなど、文書作成のプロジェクトを円滑に進めていく事ができます。

僕はGitHubの人じゃないですが、この記事で紹介する GitHub pages は、HTMLを覚えなくても簡単なマークダウンで作成できて、テーマを設定によって、見やすい書式へ自動変換される優れたものです。 


### レイアウト設定

マークダウンの先頭に、次のコマンドをセットすることで、レイアウトを設定できます。このレイアウトの設定ファイル`default`は `__layouts/default.html` に配置されます。　この設定によって画面のデザインを変更する事ができます。

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



###

# [](#header-1)Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## [](#header-2)Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.


### [](#header-3)Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```


#### [](#header-4)Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.



##### [](#header-5)Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.



###### [](#header-6)Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

