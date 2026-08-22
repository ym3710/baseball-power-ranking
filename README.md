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

PL学園（大阪）は歴史的な強豪だが、現在は野球部が実質的に活動休止中で、上記ソースに該当ページが見当たらなかったため見送っている。

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

理想は「甲子園に出場した全ての高校」だが、これを今までと同じ精度(1校ずつ個別に裏付けを取る)でやるには数百〜1000校規模になり非現実的。また試した結果、複雑な組み合わせ表(トーナメント表)を自動で正確に読み取ることには技術的な限界があることも分かった。そのため、直近の出場校一覧(信頼できる形式で取得可能)から頻出校・知名度のある学校を優先して追加し、50校前後を目安に、1校ずつ確実に検証しながら拡張していく方針にしている。

## 経緯

もともとportfolio-site（個人の自己紹介サイト）内のページとして作り始めたが、このサイトの想定読者は自分自身ではなく高校野球の選手・関係者であり、個人の自己紹介ページとは切り離すべきと判断して独立リポジトリに移した。
