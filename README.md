# 甲子園パワーランキング

春夏の甲子園(高校野球全国大会)実績だけを使って独自にスコア化した、非公式のパワーランキングサイト。

**公開URL:** https://ym3710.github.io/koshien-power-ranking/

学力データは意図的に含めていない。慶應義塾・早稲田実業のような附属校は、卒業生の多くが内部進学で系列大学に進むため、東大合格者数などで比較すると不公平になる。この問題を避けるため、純粋に甲子園の実績だけでスコア化している。

## 使用技術

- HTML / CSS / JavaScript（フレームワークなし、静的ファイルのみ）
- データは`koshien-data.js`（歴代通算）と`koshien-recent-data.js`（直近10年、年別）に分離
- GitHub Pages（静的サイトホスティング）

## スコアの計算式

```
パワースコア = 優勝回数 × 10 + 出場回数 × 2 + 通算勝利数 × 1
```

「直近10年で見る」モードでは、上記と同じ式を、選んだ開始年以降のデータだけで再計算する。

## データ出典

各校の春夏別の出場回数・優勝回数・勝利数は、**バーチャル高校野球（朝日新聞社×ABCテレビ運営、大会主催者側の公式データ）**の各校ページを出典としている（2026年8月時点のスナップショット）。

- 大阪桐蔭: [baseball.yahoo.co.jp/hsb/teams/20092](https://baseball.yahoo.co.jp/hsb/teams/20092/top)
- 智辯和歌山: [baseball.yahoo.co.jp/hsb/teams/20094](https://baseball.yahoo.co.jp/hsb/teams/20094/top)
- 横浜: [baseball.yahoo.co.jp/hsb/teams/20016](https://baseball.yahoo.co.jp/hsb/teams/20016/top)
- 東海大相模: [baseball.yahoo.co.jp/hsb/teams/20051](https://baseball.yahoo.co.jp/hsb/teams/20051/top)
- 慶應義塾: [baseball.yahoo.co.jp/hsb/teams/20054](https://baseball.yahoo.co.jp/hsb/teams/20054/top)
- 中京大中京: [baseball.yahoo.co.jp/hsb/teams/20025](https://baseball.yahoo.co.jp/hsb/teams/20025/top)
- 東邦: [baseball.yahoo.co.jp/hsb/teams/20056](https://baseball.yahoo.co.jp/hsb/teams/20056/top)
- 龍谷大平安: [baseball.yahoo.co.jp/hsb/teams/20193](https://baseball.yahoo.co.jp/hsb/teams/20193/top)
- 仙台育英: [baseball.yahoo.co.jp/hsb/teams/20147](https://baseball.yahoo.co.jp/hsb/teams/20147/top)
- 履正社: [baseball.yahoo.co.jp/hsb/teams/20119](https://baseball.yahoo.co.jp/hsb/teams/20119/top)
- 広陵: [baseball.yahoo.co.jp/hsb/teams/20170](https://baseball.yahoo.co.jp/hsb/teams/20170/top)
- 明徳義塾: [baseball.yahoo.co.jp/hsb/teams/20041](https://baseball.yahoo.co.jp/hsb/teams/20041/top)
- 帝京: [baseball.yahoo.co.jp/hsb/teams/20145](https://baseball.yahoo.co.jp/hsb/teams/20145/top)
- 日大三: [baseball.yahoo.co.jp/hsb/teams/20014](https://baseball.yahoo.co.jp/hsb/teams/20014/top)
- 花巻東: [baseball.yahoo.co.jp/hsb/teams/20077](https://baseball.yahoo.co.jp/hsb/teams/20077/top)
- 花咲徳栄: [baseball.yahoo.co.jp/hsb/teams/20249](https://baseball.yahoo.co.jp/hsb/teams/20249/top)
- 報徳学園: [baseball.yahoo.co.jp/hsb/teams/20030](https://baseball.yahoo.co.jp/hsb/teams/20030/top)
- 智辯学園: [baseball.yahoo.co.jp/hsb/teams/20171](https://baseball.yahoo.co.jp/hsb/teams/20171/top)
- 神村学園: [baseball.yahoo.co.jp/hsb/teams/20070](https://baseball.yahoo.co.jp/hsb/teams/20070/top)
- 山梨学院: [baseball.yahoo.co.jp/hsb/teams/20229](https://baseball.yahoo.co.jp/hsb/teams/20229/top)
- 東洋大姫路: [baseball.yahoo.co.jp/hsb/teams/20141](https://baseball.yahoo.co.jp/hsb/teams/20141/top)
- 沖縄尚学: [baseball.yahoo.co.jp/hsb/teams/20069](https://baseball.yahoo.co.jp/hsb/teams/20069/top)
- 佐野日大: [baseball.yahoo.co.jp/hsb/teams/20155](https://baseball.yahoo.co.jp/hsb/teams/20155/top)
- 健大高崎: [baseball.yahoo.co.jp/hsb/teams/20285](https://baseball.yahoo.co.jp/hsb/teams/20285/top)
- 京都国際: [baseball.yahoo.co.jp/hsb/teams/20425](https://baseball.yahoo.co.jp/hsb/teams/20425/top)
- 聖光学院: [baseball.yahoo.co.jp/hsb/teams/20008](https://baseball.yahoo.co.jp/hsb/teams/20008/top)
- 青森山田: [baseball.yahoo.co.jp/hsb/teams/20003](https://baseball.yahoo.co.jp/hsb/teams/20003/top)
- 早稲田実業: [baseball.yahoo.co.jp/hsb/teams/20115](https://baseball.yahoo.co.jp/hsb/teams/20115/top)
- 関東第一: [baseball.yahoo.co.jp/hsb/teams/20192](https://baseball.yahoo.co.jp/hsb/teams/20192/top)
- 明豊: [baseball.yahoo.co.jp/hsb/teams/20046](https://baseball.yahoo.co.jp/hsb/teams/20046/top)
- 鶴岡東: [baseball.yahoo.co.jp/hsb/teams/20282](https://baseball.yahoo.co.jp/hsb/teams/20282/top)
- 東海大菅生: [baseball.yahoo.co.jp/hsb/teams/20114](https://baseball.yahoo.co.jp/hsb/teams/20114/top)
- 済美: [baseball.yahoo.co.jp/hsb/teams/20040](https://baseball.yahoo.co.jp/hsb/teams/20040/top)
- 広島商: [baseball.yahoo.co.jp/hsb/teams/20036](https://baseball.yahoo.co.jp/hsb/teams/20036/top)
- 松山商業: [baseball.yahoo.co.jp/hsb/teams/19525](https://baseball.yahoo.co.jp/hsb/teams/19525/top)
- 浦和学院: [baseball.yahoo.co.jp/hsb/teams/20012](https://baseball.yahoo.co.jp/hsb/teams/20012/top)
- 常総学院: [baseball.yahoo.co.jp/hsb/teams/20053](https://baseball.yahoo.co.jp/hsb/teams/20053/top)
- 天理: [baseball.yahoo.co.jp/hsb/teams/20031](https://baseball.yahoo.co.jp/hsb/teams/20031/top)
- 敦賀気比: [baseball.yahoo.co.jp/hsb/teams/20194](https://baseball.yahoo.co.jp/hsb/teams/20194/top)
- 作新学院: [baseball.yahoo.co.jp/hsb/teams/20232](https://baseball.yahoo.co.jp/hsb/teams/20232/top)
- 高松商業: [baseball.yahoo.co.jp/hsb/teams/20377](https://baseball.yahoo.co.jp/hsb/teams/20377/top)
- 桐蔭学園: [baseball.yahoo.co.jp/hsb/teams/20129](https://baseball.yahoo.co.jp/hsb/teams/20129/top)
- 大体大浪商: [baseball.yahoo.co.jp/hsb/teams/19299](https://baseball.yahoo.co.jp/hsb/teams/19299/top)
- 秋田商業: [baseball.yahoo.co.jp/hsb/teams/20006](https://baseball.yahoo.co.jp/hsb/teams/20006/top)
- 銚子商業: [baseball.yahoo.co.jp/hsb/teams/20081](https://baseball.yahoo.co.jp/hsb/teams/20081/top)
- 静岡商業: [baseball.yahoo.co.jp/hsb/teams/20143](https://baseball.yahoo.co.jp/hsb/teams/20143/top)
- 県岐阜商: [baseball.yahoo.co.jp/hsb/teams/20023](https://baseball.yahoo.co.jp/hsb/teams/20023/top)
- 倉敷商: [baseball.yahoo.co.jp/hsb/teams/20210](https://baseball.yahoo.co.jp/hsb/teams/20210/top)
- 二松学舎大付: [baseball.yahoo.co.jp/hsb/teams/20354](https://baseball.yahoo.co.jp/hsb/teams/20354/top)
- 佐賀北: [baseball.yahoo.co.jp/hsb/teams/20187](https://baseball.yahoo.co.jp/hsb/teams/20187/top)（春の記録が未掲載のため春は0回として扱う）
- 高知商業: [baseball.yahoo.co.jp/hsb/teams/20149](https://baseball.yahoo.co.jp/hsb/teams/20149/top)
- 沖縄水産: [baseball.yahoo.co.jp/hsb/teams/19477](https://baseball.yahoo.co.jp/hsb/teams/19477/top)
- 八戸学院光星: [baseball.yahoo.co.jp/hsb/teams/20109](https://baseball.yahoo.co.jp/hsb/teams/20109/top)
- 習志野: [baseball.yahoo.co.jp/hsb/teams/20224](https://baseball.yahoo.co.jp/hsb/teams/20224/top)
- 済々黌: [baseball.yahoo.co.jp/hsb/teams/20305](https://baseball.yahoo.co.jp/hsb/teams/20305/top)
- 東北(宮城): [baseball.yahoo.co.jp/hsb/teams/20005](https://baseball.yahoo.co.jp/hsb/teams/20005/top)
- 尽誠学園: [baseball.yahoo.co.jp/hsb/teams/20039](https://baseball.yahoo.co.jp/hsb/teams/20039/top)
- 佐賀商業: [baseball.yahoo.co.jp/hsb/teams/20102](https://baseball.yahoo.co.jp/hsb/teams/20102/top)
- 中央学院: [baseball.yahoo.co.jp/hsb/teams/20406](https://baseball.yahoo.co.jp/hsb/teams/20406/top)
- 三重: [baseball.yahoo.co.jp/hsb/teams/20132](https://baseball.yahoo.co.jp/hsb/teams/20132/top)
- 熊本工業: [baseball.yahoo.co.jp/hsb/teams/20045](https://baseball.yahoo.co.jp/hsb/teams/20045/top)
- 桜美林: [baseball.yahoo.co.jp/hsb/teams/19154](https://baseball.yahoo.co.jp/hsb/teams/19154/top)
- 日大山形: [baseball.yahoo.co.jp/hsb/teams/20136](https://baseball.yahoo.co.jp/hsb/teams/20136/top)
- 宇部商業: [baseball.yahoo.co.jp/hsb/teams/20063](https://baseball.yahoo.co.jp/hsb/teams/20063/top)
- 駒大苫小牧: [baseball.yahoo.co.jp/hsb/teams/20002](https://baseball.yahoo.co.jp/hsb/teams/20002/top)
- 星稜: [baseball.yahoo.co.jp/hsb/teams/20058](https://baseball.yahoo.co.jp/hsb/teams/20058/top)
- 前橋育英: [baseball.yahoo.co.jp/hsb/teams/20272](https://baseball.yahoo.co.jp/hsb/teams/20272/top)
- 常葉大菊川: [baseball.yahoo.co.jp/hsb/teams/20164](https://baseball.yahoo.co.jp/hsb/teams/20164/top)
- 秀岳館: [baseball.yahoo.co.jp/hsb/teams/20376](https://baseball.yahoo.co.jp/hsb/teams/20376/top)
- 木更津総合: [baseball.yahoo.co.jp/hsb/teams/20213](https://baseball.yahoo.co.jp/hsb/teams/20213/top)
- 東海大甲府: [baseball.yahoo.co.jp/hsb/teams/20017](https://baseball.yahoo.co.jp/hsb/teams/20017/top)
- 松商学園: [baseball.yahoo.co.jp/hsb/teams/20085](https://baseball.yahoo.co.jp/hsb/teams/20085/top)
- 帯広農業: [baseball.yahoo.co.jp/hsb/teams/19022](https://baseball.yahoo.co.jp/hsb/teams/19022/top)
- 岡山理大付: [baseball.yahoo.co.jp/hsb/teams/20035](https://baseball.yahoo.co.jp/hsb/teams/20035/top)
- 大分商業: [baseball.yahoo.co.jp/hsb/teams/20327](https://baseball.yahoo.co.jp/hsb/teams/20327/top)
- 高知: [baseball.yahoo.co.jp/hsb/teams/20100](https://baseball.yahoo.co.jp/hsb/teams/20100/top)
- 鹿児島実業: [baseball.yahoo.co.jp/hsb/teams/20048](https://baseball.yahoo.co.jp/hsb/teams/20048/top)
- 樟南: [baseball.yahoo.co.jp/hsb/teams/20106](https://baseball.yahoo.co.jp/hsb/teams/20106/top)
- 浜松商業: [baseball.yahoo.co.jp/hsb/teams/19233](https://baseball.yahoo.co.jp/hsb/teams/19233/top)

PL学園（大阪）は歴史的な強豪だが、現在は野球部が実質的に活動休止中で、上記ソースに該当ページが見当たらなかったため見送っている（2回探したが両方とも該当ページなし）。

合計値(出場・優勝・勝利)はデータに直接持たず、`index.html`側で春+夏の数値から毎回計算している（同じ値を2箇所に書くとズレの原因になるため）。

**注意: Wikipediaは出典として使っていない。** 誰でも編集できて信頼性が担保されないため。優勝年など個別の事実確認は、学校の公式サイトか、編集責任のある新聞社・ニュースサイトの記事のみを使っている。

## 「直近10年で見る」機能のデータ出典(`koshien-recent-data.js`)

パイロット5校のみ、年別の出場・勝敗を`koshien-recent-data.js`に持たせている。優勝年は以下の一次情報・報道で個別に裏付けを取った。

- 大阪桐蔭 2022年春優勝: [日本経済新聞](https://www.nikkei.com/article/DGXZQODH315DD0R30C26A3000000/)（2026年の「4年ぶり5度目の優勝」表現から逆算）
- 智辯和歌山 2021年夏優勝: [中日スポーツ](https://news.yahoo.co.jp/articles/56a40227d3df5d741a1feba161279f52fec0e183)、[スポーツ報知](https://news.yahoo.co.jp/articles/d1f077d0d48eebc54b87fa06af5ea44b28e6522b)
- 横浜 2025年春優勝: [神奈川新聞(カナロコ)](https://www.kanaloco.jp/sports/baseball/hsbaseball/article-1160151.html)
- 中京大中京: [学校公式サイトの部史年表](https://www.chukyo.ed.jp/information/history01.html)で、直近の優勝は2009年が最後(2016年以降の優勝なし)と確認
- 龍谷大平安: 2016年以降の優勝なし。2024年に京都国際が68年ぶりの京都勢優勝と報じられている（[高校野球ドットコム](https://www.hb-nippon.com/articles/2440)）ことから、1956年の平安以来優勝していないことを裏付け

上記以外の年(優勝以外の出場)は、バーチャル高校野球の年別成績ページをベースにしているが、決勝の勝敗判定だけは上記の個別裏付けを優先している（年別ページ側の「決勝」表記に漏れ・誤りがあったため）。

2026年でまだ結果が確定していない出場は含めていない。他9校の年別データは未整備（一覧では「直近10年データ準備中」と表示）。

## 掲載校の範囲について

理想は「甲子園に出場した全ての高校」だが、これを今までと同じ精度(1校ずつ個別に裏付けを取る)でやるには数百〜1000校規模になり非現実的。また試した結果、複雑な組み合わせ表(トーナメント表)を自動で正確に読み取ることには技術的な限界があることも分かった。

そのため「全国全校」を最終的な目標としつつ、1回のセッションでは現実的な数十校ずつ、知名度・頻出度の高い学校から優先して1校ずつ確実に検証しながら継続的に拡張していく方針にしている。一気に完成させるものではなく、少しずつ育てていくデータベース。

## 経緯

もともとportfolio-site（個人の自己紹介サイト）内のページとして作り始めたが、このサイトの想定読者は自分自身ではなく高校野球の選手・関係者であり、個人の自己紹介ページとは切り離すべきと判断して独立リポジトリに移した。
