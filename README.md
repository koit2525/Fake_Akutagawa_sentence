# AIによる芥川龍之介風文章の自動生成

## プロジェクト概要
このプロジェクトではAIによる芥川龍之介風文章の自動生成を行います。
具体的には[rinna株式会社](https://rinna.co.jp/)よりオープンソースとして公開されている"GPT-2事前学習モデル"を、青空文庫から取得した芥川龍之介の小説を学習データとしてファインチューニングを実施します。<br>
そして芥川の代表作である「羅生門」と「蜘蛛の糸」の文頭と彼の晩年の名言から、ファインチューニングされたモデルが芥川風の文章を生成できるのかを実験します。<br>
また本プロジェクトの実行環境としてはGoogle Colaboratory Proを利用しています。

## 実験結果

-------「ある日の暮方の事である。」から生成した芥川龍之介風文章-------<br>
ある日の暮方の事である。
 と云う風な事を言つた。
わたしはその時、耳をつんざくばかりの、可笑しいと思つた。
あの調子だから、一々のを鳴らしながら、わたしの言ひつけを聞かないかも知れない。
さう思いながら、わたしは口をとざした。
いつか、あの悪夢から醒めたように、わたしはもう一度この調子で、わたしの言ひつけを言ふ真似事をしたいと思つたからだ。

-------「ある日の事でございます。」から生成した芥川龍之介風文章-------<br>
あある日の事でございます。
 」と云つた。
云つた後も、何度もかう考へた。
「兎に角、信輔は、どうして、今だ信輔の決心は、弟には通じないのであろう? 何にしても、彼の決心は、弟には、容赦がないのに相違ない。
それに、どうして、こんなにも、信輔を憎む気になるのでございましょう。
」信輔は、一瞬間、口角に、髭の生えた、可笑しさを含んだ微笑を感じた。
が、同時に又、複雑な心もちが、込み上げて来た。
それは、疑うのを誤って、自分を殺さなかつた弟に対する、彼の復讐心を、復讐しようとする彼の心が、知らず知らず、そうして、その時は、燃えている、熱した、あの黒煙と同じやうな不快な、そんな忌まわしい、忌まわしい、考えに変らざるを得なかったからである。

-------「僕の将来に対する唯ぼんやりとした不安」から生成した芥川龍之介風文章-------<br>
僕の将来に対する唯ぼんやりとした不安或はこの不安にいつも脅かされ、絶えず怯えながら、しかもそれと共にそれと同時に愉快な悦びを感じない訣には行かない僕の心の問題である。
けれども将来に対する不安は僕を更に苦しめずには措かない。
僕の僕であるためにこの不相変将来に対する不安ばかり生じているのである。
僕の将来に対する不安は「どうにでもなれ」と云う力の根源に違いない。
「どうにでもなれ」と云う力の源に違いないのは、単に僕が「どうにでもなれ」と云う勇気を持つてゐない為だ。
それを「どうにでもなれ。
さうしてしまへば」と云ふ力の源にすれば、僕は力の無い人間になり兼ねない。
「どうにでもなれ力の源になれば」と云ふ勇気は勿論この「どうにでもなれ力の源になれば」と云ふ力を生む為に必要である。
けれどもそれは同時に「どうにもならざる力の源になれば」と云ふ力を生んで来ない。
この「どうにもならざる力の源にならざる」が僕の困るところである。

## 結果に対する考察
「芥川風文章とは何か」を明確に定義することはできません。
そのためこの結果が良いのか悪いのかを定量的に表現することもできません。
しかし３例目などは「得体の知れない不安感への苦悩」が、ぼんやりと私には伝わってくる文章です。
これは比較的良い結果と言えるのではないでしょうか。
一方で２例目の「」と云つた。」など日本語文の体を成していない部分も見受けられます。

GPT-3などさらに大規模なモデルを用いて、同様の実験を行なった場合は、どのような結果になるのか大変興味深いです。

## 備考
***** train metrics *****

epoch                    =       10.0

train_loss               =     2.3476

train_runtime            = 0:36:11.06

train_samples            =        224

train_samples_per_second =      1.032

train_steps_per_second   =      1.032


## 参考
[GPT-2をファインチューニングしてニュース記事のタイトルを条件付きで生成してみた。](https://qiita.com/m__k/items/36875fedf8ad1842b729)
