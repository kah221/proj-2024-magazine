# 序章

この文章は、私が作ったカバンの設計から製作までをまとめてみたものです。前提として、私は服の型紙を引く能力などはなく、家庭科の成績もそこまで良くなかった人間なので、様々に至らない点がある可能性は十分にありますが、ご了承ください。  
さて、では記録の前に、このカバンの開発の経緯について紹介したいと思います。弊部、島根大学ものづくり部PimではPCを持ち歩いている方が非常に多く、スマートフォンよりもPCのほうが利用する頻度がずっと高いので、家にスマートフォンを忘れてくるという事象もしばしば見られるほどです。しかしながら、PCは当然のことながらも持ち運び等の利便性に劣ります。更に手で持って輸送するわけにもいかないので、リュックサックに入れており、取り出すまで時間がかかってしまうこともあります。そこで、PCを気軽に、様々な形態で持ち運ぶことができて、必要に応じてすぐに取り出すことができるようなカバンがあったら良いなという思想の元、カバンを開発することに思い至った次第であります。

# 設計

## 大まかな形の決定

PCカバンに必要な機能を洗い出し、それを解決する為にどのような部品が必要なのか検討する。

| 必要な機能 | それを実現する部品 |
| :---- | :---- |
| 肩からかけられる | 肩紐をつける |
| 防水 | 撥水・防水機能のある布を使う |
| 充電ケーブル入れ | 外部的に追加できるポケット |
| 長時間かけていられる | 頑丈なベルトを肩紐に利用 |
| 手提げできる | 肩紐の形を工夫or手提げを実装 |
| 変形の防止 | 硬めのスポンジゴムを入れる |
| コード等を無くしにくい | 布地の色を明るくする |
|  |  |

## 仕様の決定

当たり前のこと過ぎて上の表には書いていませんが、このカバンの一番の目的はノートPCを持ち運ぶことです。それに従ってカバンの仕様決定にはノートPCがどのようなものであるかを把握して置かなければなりません。なので、14型までのノートPCのサイズと重量を調べてまとめ、表にしてみて最大値を取っていくことによって大体のノートPCに対応できるようにしました。一般的なノートPCの中で15.6型という比較的大きいノートPCもありましたが、今回はそこまでのサイズに適応すると14型ですら長さが5cmほど余ってしまうため、断念しました。IdeaPadやSurface、Vaio、HP、ThinkPad、LAVIEの14型ノートPCのサイズをすべて並べてみた結果、LAVIE N14がもっともサイズが大きいことが判明しました。なので、このPCを基準にサイズを設計していきます。N14は326\*226\*20mm(小数点以下四捨五入)のサイズであるので、カバンの基本の型紙にそのサイズを適応していきます。  
他の要件を満たす方法も考えていきます。まず、防水の機能です。この実現は防水の布を使います。ここで重要なのは撥水では不十分であるということです。PCが水没するとかなりの損害になります。そのため、しっかりと防水であるものを選びます。私は帆布カバン信者なので、ラミネートされている帆布を使うことにしました。ちなみにお金に余裕があるなら、パラフィン加工(簡単に言うとロウを染み込ませた)の帆布などは質感も良くなります。最後に硬めのスポンジゴムについてですが、これは正直に言うと実装をためらっています。なぜならばスポンジゴムを固定しておくために裏地の実装が必須になってくるので、費用が裏地の分とスポンジゴムとで多くかかってしまうからです。カバン一つに対して幾らまで出せるかを検討し、量産時に購入する布地や部品の値段を加味することで、実装するかの最終的な判断をすることにします。

## 型紙の作成

カバンをどのような形・サイズにするかが決まったので、型紙を引く段階に移ります。型紙を引くと言いつつも直方体の形で、私がよく使っているテンプレート(fig.1)があるので、そちらに今回のサイズを適応する形にしたいと思います。しかし、今回のカバンの厚みは20mmと非常に小さいので、fig.1にある{厚み/2}というものが非常に小さくなります。そこで、今回は片側からカバンの横の部分の布を提供する形に変更することにします。ということで、完成した型紙が(fig.2)です。ちなみに直方体ならば、天面のない一般的な直方体の展開図のように、側面に使用する布として底面に使用する布の余りが利用できると思われるかもしれませんが、それではいくらか都合の悪いことが発生します。一つは地の目の話です。布は巻いてある向きとそれに垂直な向きがあります。巻いてある向きを地の目と言い、この方向には強くできていることがほとんどです。この布の向きをカバンの上下に設定することで布の強い性質を出せるのですが、そのような布の取り方をすると、側面か前後面のどちらかが地の目になることができないのです。もう一つの都合の悪い点は、布の取り方です。そのような布の取り方をすると、余った布の中で取れる長方形のサイズが小さくなることがわかります。これによって他の用途に使いにくい布が発生してロスになってしまうので、このような布の取り方を控えているわけです。  
さて、カバンに使う布をどのような形に取るかは決定したところですが、これで型紙は完成ではありません。縫い代というものをつけることで、ようやく縫えるようになります。今回は裏地を張ることも考慮に入れたいため、縫い代は20mmに設定しておきました。一般的な縫い代は10mmですが、今回は裏地をつけない可能性があり、生地の端処理を三つ折りにて行いたいため20mmを採用しました。端処理の方法は他にもあり、例えば布テープで覆ってしまう方法や、ロックミシンをかける方法、などがありますが、一番費用が安上がりなので折り込んでしまう方法を取りました。

## 肩紐の仕様の決定

続いて肩紐の実装について決めていきます。今回、肩紐はカバンから4つのDかん等を出して、肩紐についたナスカンでそのうち2つを選択するという方式をとることにします。私が以前に作成したメッセンジャーバッグは側面の布に肩紐が縫い付けられていたのですが、これだと用意に肩紐を交換することができないほか、側面が引っ張られるので底面にかかっている重量は底面と側面の布の縫い目を経由して肩紐にかかることになります。そのため、耐久性に不安があったほか、底面の側面近くが上に持ち上がることで、中央部にシワが寄りやすくなってしまうことがあったため、それらを解消するために、底面から布が上向きに地の目で続いている場所にDかん等を設置することで、耐久性や形状の保持が期待できると考え、このような方式にしました。

# 試作

## 型紙の検証

先ほど引いた型紙が正しく自分の想像している形になるかどうか、形に縫うことができるような構造であるかどうかを検証します。検証といっても図形と向き合っていても仕方がないので、私はペーパークラフトを用いて検証します。大抵は1/2スケール(スケールは手元の紙の大きさに合わせて調整する)に紙を測って型紙通りに切り取り、想定している折り目をつけてきちんとカバンの形になるかを検証します。この際にきちんと確認して置かなければならないのは、底に穴などがないかということです。この時点で底や壁の接合部分に穴があると、カバンにした際にも縫い合わせるのは困難な形となってしまいます。  
次に、この手法で、縫い代があるバージョンも検証していきます。今回のようにテンプレートと違う縫い代の付け方をした際などは特に注意が必要です。ちなみに私は検証をせずに布を切ったので、長さが合わない布ができて、非常に苦労しました。というか、布を無駄にしてしまうことになりました。なので、必ず検証はしてから布に型紙を写し取るようにしましょう。

## 試作を作る

検証の終了した型紙ができたら、型紙に従って布に印を付けていきます。今回の場合などもそうですが、実寸大の型紙を用意する必要はありません。どこが何cmで四角形を書けばよいかわかっていれば、型紙を布に当てて書く必要はなく、むしろその方が地の目の向きを意識して布を使うことができます。  
これによって布に線を引いたらそれに沿って布を切断し、端の処理を適切にし、縫い合わせていきます。このあたりは家庭科の知識なので、わからないことやできないことがあれば、当該の教科書を参照するなどしてください。カバンを一つ作るだけなら、これに好みの肩紐をつけるだけで完成でございます。
