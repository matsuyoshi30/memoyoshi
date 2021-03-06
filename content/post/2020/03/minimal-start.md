+++
title = "小さいことから始める"
date = 2020-03-21T17:25:29+09:00
tags = ["letters"]
draft = false
toc = false
backtotop = false
+++

COVID-19 の流行が収まる気配が全く無い。

本日は友人の結婚式に参列する予定だったのだが、3週間ほど前に友人から「コロナウイルスの影響で、結婚式や二次会を8月に延期する」と連絡があった。
1ヶ月後にはまた別の友人の結婚式（二次会）が2件予定されているのだが、問題なく開催されるかどうか怪しい。

GitHub の Trend は COVID-19 関係のリポジトリが多くを占めるようになり、世界的な流行がどんどん拡大していることを示している。
自作の[CLI ツール](https://github.com/matsuyoshi30/go-trendrepo)で最近作成されたリポジトリかつスター数が多いものをたまに覗いてみるのだが、
ここ最近は COVID-19 関連が多い。

先日、東京都が公開している[新型コロナウイルス感染症対策サイト](https://stopcovid19.metro.tokyo.lg.jp/)が話題になった。
これは今 Trend にのっているリポジトリと同様に、サイトの内容が GitHub に MIT ライセンスで公開されており、issue や pull request も受け付けていて、3/21時点で192人の contributor がいる（[リポジトリ](https://github.com/tokyo-metropolitan-gov/covid19)）。
今まで知らなかったのだが、ヤフーで社長を務めた宮坂学氏が副都知事であることが大きいようだ。
IT に精通している人間が組織のトップ近くにいると、スピード感を持ってこういった対応ができるという好例だと思う。

話題の中で、超天才プログラマーとしても非常に有名で台湾のデジタル担当大臣である唐鳳（オードリー・タン）からの pull request が注目を集めた。
東京都のコロナ対策サイトに海外の大臣が直接修正を加えるという事態に Twitter 等では大きな盛り上がりを見せた。

唐鳳氏の今回の pull request は繁体字の1文字修正のみであり、「1文字の修正で注目が大きすぎるのではないか」といった意見もあったが、自分はそう思わなかった。
むしろこれを見て pull request に対するハードルが大きく低くなり、どんどん pull request を出していこうという考えになった。

この出来事の他にもいろいろあり、最近 pull request に対する自分の姿勢が変わってきている。
前置きはここまでにして、ここから pull request に対する今の自分の姿勢を示しておく。
技術者を自称する人間の一般的な姿勢だ思うので、この記事は初心者と初心者の頃の自分向けであることを前もって断っておく。

## 自分でハードルを高くしない

僕は普段業務でコードを書くことはほとんどない。休日に自分の興味のある分野や言語についていろいろ調べつつ、週末プロジェクト的にコードを書いている。
ネットでは『強い』方々の会話や意見を読み、「こうなりたいな〜」などとぼんやり考えていて、同じように自分の意見を述べたりするのはまだ早いとか考えている。

pull request に対してもおんなじだ。
むしろ、常日頃コードを書いていて自分より知識もスキルもある人のプロジェクトに対して、僕が pull request なんて出していいものなのだろうか、と考えていた。

そんなとき、前回の記事でも述べた[自作の Hugo Theme](https://github.com/matsuyoshi30/harbor)を Hugo 公式のテーマ紹介に載せてもらい、スターを貰った。
少しあとには pull request が飛んできて、内容は「 README.md に記載している config.toml の例に theme も記載しようね」というものだった。
自分のリポジトリに pull request を貰ったのは初めてで嬉しくなり、興奮して Thank you!!! って返せばいいのかな、なんて返答例を調べたりした（結局はコメントなしでマージしたが）。

このとき、 pull request を貰う側の気持ちが少し分かったような気がする。
自分のプロジェクトに存在する間違いや追加したほうが良い機能について、他の人が気付いて修正依頼を投げてくれるというのはある意味「他者から承認されている」状態だ。
他者がわざわざ時間を割いて、見ず知らずの自分に対して能動的に意見を伝えようとしてきているという事実は嬉しい。

pull request を投げるとき、自分の中でハードルを高くしてはいけない。
自分の意見を能動的に他者に伝えること自体にまず価値があるし、自分の意見が相手にとって大きいか小さいかは相手が判断することだ。
少なくとも「他の人間の言うことなんて全部無視や！」なんて考えてる人はリポジトリを公開しないし、したとしても README にでっかく書いている。
そうでない限りはバシバシ pull request を出していこう。

## 間違うことで学ぶ

前は「 pull request なんて出しても、その内容が間違えたりしたら相手の時間を無駄にしてしまう」という考えがあった。
この考えがすべて誤っているとは思わないが、仮に pull request の内容が間違っていたとしても、その時点で自分が正しいと思っていれば迷わず出すべきだ。
それが間違っているかどうかは自分で抱え続けても判断できないし、むしろ間違いが指摘されれば「それが間違いである」という内容が明示的に残ることで、
自分と同じように間違う可能性のある人間に対するガイドとなる。

もちろんドキュメントを読まずに pull request を出し、その内容がドキュメントを読めば間違いだとわかる場合はどうかと思うが、程度の問題だと思う。
読んでも分かりづらかったり、そもそもその内容が記載されている箇所に辿り着きづらい場合は、それ自体を修正しましょうというきっかけにもなる。

「間違っていたらどうしよう」なんて考えは誰のためにもならないので、間違わないことに注力しつつも「どんどん間違えていこう」という気持ちに変えよう。

話は少し違うけど、[ここ](http://blog.practical-scheme.net/shiro/20161229-100-rejections)で書かれていることも少しばかりは関連すると思う。

## 同じところに留まらない

一個 pull request を出すと、「もっと貢献できないかな」「他にも貢献できる場所は無いかな」という気持ちになる。
けど、既に発行されている issue を見ると、今の自分では解決できなさそうな問題ばかりが並んでいたりする。

そしたら次は、その問題が自分で解決できるようになるまで学習し続けることが大事だ。
もちろんこれまで出した pull request と同じような貢献の形に意味が無いなんてことは無いが、いつまでも同じようなことをしていても面白くない。

pull request をモチベーションの一つにすることで、自分を成長させていきたい。
なお、僕は今 pull request し始めたばかりなので、こんなことを言っておいてその段階にいない。
他の人に面と向かってこういうことが言えるよう、今後自分で実践しなければ。。。

## 結

先にも述べたが、問題の大小は基本的に当事者にならないと分からない。 pull request を出すことでまず当事者になる第一歩を踏み出すことが出来ると思う。
それが結局小さいことだったとしても、まずは始めないことには形にならないという意識を持ち続けたい。最初の一歩で大きなことを成し遂げられるほど自分は天才ではないことを自覚する。

今日は勝手にロールモデルにしたいと思っている ohbarye 氏の [goofi](https://github.com/ohbarye/goofi)に [pull request](https://github.com/ohbarye/goofi/pull/277) を出して、無事にマージされた。
内容は「`target="_blank"`のリンクは`rel="noopener"`を付ける」というだけ。これまで TypeScript や Next.js は触ったことが無いが、 pull request をきっかけにこのリポジトリで勉強したいと思う。
pull request はいい事だらけである。

## 見ておくと助かるもの

- 心構え
    - [Oss貢献超入門](https://www.slideshare.net/shigemk2/oss-78585757)
    - [貢献できるOSSの見つけ方 / How to find "Good First Issues"](https://speakerdeck.com/ohbarye/how-to-find-good-first-issues)
    - [続・貢献できるOSSの見つけ方 / How to find "Good First Issues" part 2](https://speakerdeck.com/ohbarye/how-to-find-good-first-issues-part-2)
    - [貢献できるOSSの見つけ方 -完結編- / How to find "Good First Issues" Final](https://speakerdeck.com/ohbarye/how-to-find-good-first-issues-final)
-  issue 探し
    - [goofi](https://goofi.now.sh/)
    - [firstcontributions](https://firstcontributions.github.io/)
    - [GitHub help wanted](http://github-help-wanted.com/)
    - [trends](https://trends.now.sh/)