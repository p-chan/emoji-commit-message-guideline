# emoji-commit-message-guideline

GitHubにおいて「コミットメッセージは英語で書くべき」というのはもはやデファクトになりつつある。

しかし、日本人のみでプロジェクトを進行する場合、英語で統一するのは無理があると思う。  
基本的に、日本人中心でリポジトリ運営を行う場合、日本語でコミットメッセージを書くべきだ。  
ただし、世界に向けたOSSである場合はこの限りではない。

<small>メインのコミッターだけでなく、たまにプルリクをくれる人や、Issueを建ててくれる人などのことを考えて使用言語を決めるべきである。</small>

<blockquote class="twitter-tweet" lang="ja"><p lang="ja" dir="ltr">コミットメッセージを英語で書いてたのに、途中で英語力足りなくなって日本語になっちゃったり、他の人が日本語でIssue立てたりして、複数言語が混ざり合うの、うーんこのってなる。</p>&mdash; Pちゃん (@p1ch_jp) <a href="https://twitter.com/p1ch_jp/status/665602448568905728">2015, 11月 14</a></blockquote> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## 日本語コミットメッセージの問題点
先程も書いたとおり、日本人でリポジトリを運営していく場合、日本語で書くのが良いと思う。  
しかし、日本語には「動詞が最後にくる」という特徴があり、パッと見でコミットの内容が分かりづらい。
そこでベターなアプローチとして、コミットの先頭にプレフィックスを付けるというものがある。  
ここでは、絵文字をプレフィックスとしたコミットメッセージのベストプラクティスを考えたい。

## 絵文字の有用性
「絵文字とか舐めてんの？」と言われそうだけど、舐めてない。  
実際に、GitHub社が開発を進めている次世代エディタAtomの開発でも絵文字が使われているくらいには市民権を得てる。  
どうでもいいけど、日本語である`絵文字`が`emoji`として世界共通語になってるの、若干嬉しい。

## プレフィックス
増えすぎても微妙なのでとりあえず5つにした。  
GitHub上で絵文字を表示させるには`:innocent:`のように特定の文字列を`:`で囲って上げれば良い。(ちなみに:innocent:のように表示される)  

- :sparkles: `:sparkles:` - 新規追加  
- :pencil2: `:pencil2:` - 修正  
- :poop: `:poop:` - バグ修正  
- :fire: `:fire:` - 削除  
- :recycle: `:recycle:` - 整理

### おまけ
:tada: `:tada:` - Initial Commitやリリースなど

### 補足
バグに:bug:`:bug:`を使わない理由は、虫嫌いな人(ぼく)を考慮したものである。  
あと、みんなうんこ好きでしょ。

## コミットメッセージ
日本語でコミットメッセージを書くにあたって、最低限以下に気をつけたい。

### 文末に読点を付けない
ワンラインなので、読点は要らない。

```
# Bad
:poop: コメントをお気に入りできないエラーを修正。

# Good
:poop: コメントをお気に入りできないエラーを修正
```

### 体言止めにする
「〜しました」で収まればいいけど、「〜させていただきました」とか出てきた日にはWTH!!ってなりそう。
というわけで、できるだけ体言止めにしましょう。

```
# Bad
:poop: コメントをお気に入りできないエラーを修正しました

# Good
:poop: コメントをお気に入りできないエラーを修正
```

## 心がけ
- 何をしたかが分かるように心がける
- 伝わる範囲で短く書くように心がける
- ガイドラインにとらわれ過ぎないように心がける

## 参考
- [Contributing to Atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md)
- [EMOJI CHEAT SHEET](http://www.emoji-cheat-sheet.com)
- [GitHubで絵文字コミットを続けてみて有用だったEmojiまとめ](http://mzyy94.com/blog/2015/10/14/emoji-commit-message/)
- [GitHub で絵文字入りコミットメッセージを活用しているプロジェクトを調べてみた](http://pronama.azurewebsites.net/2015/06/20/github-emoji-commit-message/)
- [dannyfritz/commit-message-emoji](https://github.com/dannyfritz/commit-message-emoji)
