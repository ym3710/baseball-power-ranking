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
- 金足農: [baseball.yahoo.co.jp/hsb/teams/20184](https://baseball.yahoo.co.jp/hsb/teams/20184/top)
- 宇和島東: [baseball.yahoo.co.jp/hsb/teams/20265](https://baseball.yahoo.co.jp/hsb/teams/20265/top)
- 今治西: [baseball.yahoo.co.jp/hsb/teams/20150](https://baseball.yahoo.co.jp/hsb/teams/20150/top)
- 鳥取城北: [baseball.yahoo.co.jp/hsb/teams/20239](https://baseball.yahoo.co.jp/hsb/teams/20239/top)
- 創成館: [baseball.yahoo.co.jp/hsb/teams/20323](https://baseball.yahoo.co.jp/hsb/teams/20323/top)
- 長崎日大: [baseball.yahoo.co.jp/hsb/teams/20174](https://baseball.yahoo.co.jp/hsb/teams/20174/top)
- 国士舘: [baseball.yahoo.co.jp/hsb/teams/20082](https://baseball.yahoo.co.jp/hsb/teams/20082/top)
- 上宮: [baseball.yahoo.co.jp/hsb/teams/19313](https://baseball.yahoo.co.jp/hsb/teams/19313/top)
- 近大付: [baseball.yahoo.co.jp/hsb/teams/20219](https://baseball.yahoo.co.jp/hsb/teams/20219/top)
- 明桜: [baseball.yahoo.co.jp/hsb/teams/20231](https://baseball.yahoo.co.jp/hsb/teams/20231/top)
- 高崎商業: [baseball.yahoo.co.jp/hsb/teams/20112](https://baseball.yahoo.co.jp/hsb/teams/20112/top)
- 徳島商業: [baseball.yahoo.co.jp/hsb/teams/20151](https://baseball.yahoo.co.jp/hsb/teams/20151/top)
- 崇徳: [baseball.yahoo.co.jp/hsb/teams/19354](https://baseball.yahoo.co.jp/hsb/teams/19354/top)
- 呉港: [baseball.yahoo.co.jp/hsb/teams/19349](https://baseball.yahoo.co.jp/hsb/teams/19349/top)
- 高川学園: [baseball.yahoo.co.jp/hsb/teams/20383](https://baseball.yahoo.co.jp/hsb/teams/20383/top)
- 佐久長聖: [baseball.yahoo.co.jp/hsb/teams/20313](https://baseball.yahoo.co.jp/hsb/teams/20313/top)
- 福井商業: [baseball.yahoo.co.jp/hsb/teams/20057](https://baseball.yahoo.co.jp/hsb/teams/20057/top)
- 富山商業: [baseball.yahoo.co.jp/hsb/teams/20019](https://baseball.yahoo.co.jp/hsb/teams/20019/top)
- 小松大谷: [baseball.yahoo.co.jp/hsb/teams/19221](https://baseball.yahoo.co.jp/hsb/teams/19221/top)
- 日本航空石川: [baseball.yahoo.co.jp/hsb/teams/20236](https://baseball.yahoo.co.jp/hsb/teams/20236/top)
- 新潟明訓: [baseball.yahoo.co.jp/hsb/teams/20084](https://baseball.yahoo.co.jp/hsb/teams/20084/top)
- 日本文理: [baseball.yahoo.co.jp/hsb/teams/20018](https://baseball.yahoo.co.jp/hsb/teams/20018/top)
- 帝京長岡: [baseball.yahoo.co.jp/hsb/teams/21660](https://baseball.yahoo.co.jp/hsb/teams/21660/top)
- 近江: [baseball.yahoo.co.jp/hsb/teams/20091](https://baseball.yahoo.co.jp/hsb/teams/20091/top)
- 滋賀学園: [baseball.yahoo.co.jp/hsb/teams/20238](https://baseball.yahoo.co.jp/hsb/teams/20238/top)
- 箕島: [baseball.yahoo.co.jp/hsb/teams/20228](https://baseball.yahoo.co.jp/hsb/teams/20228/top)
- 市和歌山: [baseball.yahoo.co.jp/hsb/teams/20032](https://baseball.yahoo.co.jp/hsb/teams/20032/top)
- 佐賀学園: [baseball.yahoo.co.jp/hsb/teams/20043](https://baseball.yahoo.co.jp/hsb/teams/20043/top)
- 有田工: [baseball.yahoo.co.jp/hsb/teams/20328](https://baseball.yahoo.co.jp/hsb/teams/20328/top)
- 池田(徳島): [baseball.yahoo.co.jp/hsb/teams/20341](https://baseball.yahoo.co.jp/hsb/teams/20341/top)
- 鳴門: [baseball.yahoo.co.jp/hsb/teams/20266](https://baseball.yahoo.co.jp/hsb/teams/20266/top)
- 松山東: [baseball.yahoo.co.jp/hsb/teams/20355](https://baseball.yahoo.co.jp/hsb/teams/20355/top)
- 三本松: [baseball.yahoo.co.jp/hsb/teams/20075](https://baseball.yahoo.co.jp/hsb/teams/20075/top)
- 倉敷工業: [baseball.yahoo.co.jp/hsb/teams/20222](https://baseball.yahoo.co.jp/hsb/teams/20222/top)
- 関西(岡山): [baseball.yahoo.co.jp/hsb/teams/20064](https://baseball.yahoo.co.jp/hsb/teams/20064/top)
- 岡山東商業: [baseball.yahoo.co.jp/hsb/teams/20121](https://baseball.yahoo.co.jp/hsb/teams/20121/top)
- 広島工業: [baseball.yahoo.co.jp/hsb/teams/20309](https://baseball.yahoo.co.jp/hsb/teams/20309/top)
- 如水館: [baseball.yahoo.co.jp/hsb/teams/20065](https://baseball.yahoo.co.jp/hsb/teams/20065/top)
- 岩国: [baseball.yahoo.co.jp/hsb/teams/20037](https://baseball.yahoo.co.jp/hsb/teams/20037/top)
- 下関商業: [baseball.yahoo.co.jp/hsb/teams/20197](https://baseball.yahoo.co.jp/hsb/teams/20197/top)
- 米子東: [baseball.yahoo.co.jp/hsb/teams/19359](https://baseball.yahoo.co.jp/hsb/teams/19359/top)
- 松江商業: [baseball.yahoo.co.jp/hsb/teams/19364](https://baseball.yahoo.co.jp/hsb/teams/19364/top)
- 北照: [baseball.yahoo.co.jp/hsb/teams/20251](https://baseball.yahoo.co.jp/hsb/teams/20251/top)
- 弘前学院聖愛: [baseball.yahoo.co.jp/hsb/teams/20326](https://baseball.yahoo.co.jp/hsb/teams/20326/top)
- 盛岡大付: [baseball.yahoo.co.jp/hsb/teams/20004](https://baseball.yahoo.co.jp/hsb/teams/20004/top)
- 一関学院: [baseball.yahoo.co.jp/hsb/teams/20110](https://baseball.yahoo.co.jp/hsb/teams/20110/top)
- 学法石川: [baseball.yahoo.co.jp/hsb/teams/19083](https://baseball.yahoo.co.jp/hsb/teams/19083/top)
- 利府: [baseball.yahoo.co.jp/hsb/teams/20221](https://baseball.yahoo.co.jp/hsb/teams/20221/top)
- 秋田中央: [baseball.yahoo.co.jp/hsb/teams/19061](https://baseball.yahoo.co.jp/hsb/teams/19061/top)
- 藤代: [baseball.yahoo.co.jp/hsb/teams/20078](https://baseball.yahoo.co.jp/hsb/teams/20078/top)
- 土浦日大: [baseball.yahoo.co.jp/hsb/teams/19094](https://baseball.yahoo.co.jp/hsb/teams/19094/top)
- 文星芸大付: [baseball.yahoo.co.jp/hsb/teams/20134](https://baseball.yahoo.co.jp/hsb/teams/20134/top)
- 桐生第一: [baseball.yahoo.co.jp/hsb/teams/20011](https://baseball.yahoo.co.jp/hsb/teams/20011/top)
- 春日部共栄: [baseball.yahoo.co.jp/hsb/teams/20080](https://baseball.yahoo.co.jp/hsb/teams/20080/top)
- 拓大紅陵: [baseball.yahoo.co.jp/hsb/teams/19143](https://baseball.yahoo.co.jp/hsb/teams/19143/top)
- 創価: [baseball.yahoo.co.jp/hsb/teams/20182](https://baseball.yahoo.co.jp/hsb/teams/20182/top)
- 横浜商業: [baseball.yahoo.co.jp/hsb/teams/19165](https://baseball.yahoo.co.jp/hsb/teams/19165/top)
- 桐光学園: [baseball.yahoo.co.jp/hsb/teams/20083](https://baseball.yahoo.co.jp/hsb/teams/20083/top)
- 中越: [baseball.yahoo.co.jp/hsb/teams/20372](https://baseball.yahoo.co.jp/hsb/teams/20372/top)
- 高岡商業: [baseball.yahoo.co.jp/hsb/teams/20090](https://baseball.yahoo.co.jp/hsb/teams/20090/top)
- 金沢: [baseball.yahoo.co.jp/hsb/teams/20144](https://baseball.yahoo.co.jp/hsb/teams/20144/top)
- 日本航空(山梨): [baseball.yahoo.co.jp/hsb/teams/20086](https://baseball.yahoo.co.jp/hsb/teams/20086/top)
- 大垣日大: [baseball.yahoo.co.jp/hsb/teams/20163](https://baseball.yahoo.co.jp/hsb/teams/20163/top)
- 静岡: [baseball.yahoo.co.jp/hsb/teams/20283](https://baseball.yahoo.co.jp/hsb/teams/20283/top)
- 愛工大名電: [baseball.yahoo.co.jp/hsb/teams/20055](https://baseball.yahoo.co.jp/hsb/teams/20055/top)
- 白山(三重): [baseball.yahoo.co.jp/hsb/teams/20411](https://baseball.yahoo.co.jp/hsb/teams/20411/top)
- 立命館宇治: [baseball.yahoo.co.jp/hsb/teams/20258](https://baseball.yahoo.co.jp/hsb/teams/20258/top)
- 育英(兵庫): [baseball.yahoo.co.jp/hsb/teams/20060](https://baseball.yahoo.co.jp/hsb/teams/20060/top)
- 神港学園: [baseball.yahoo.co.jp/hsb/teams/20120](https://baseball.yahoo.co.jp/hsb/teams/20120/top)
- 和歌山東: [baseball.yahoo.co.jp/hsb/teams/20462](https://baseball.yahoo.co.jp/hsb/teams/20462/top)（夏の出場記録なし、未出場として0回扱い）
- 興国: [baseball.yahoo.co.jp/hsb_summer_local/entryteams/19303](https://baseball.yahoo.co.jp/hsb_summer_local/entryteams/19303)
- 大阪学院大: [baseball.yahoo.co.jp/hsb/teams/22243](https://baseball.yahoo.co.jp/hsb/teams/22243/top)（夏は出場なし）
- 創志学園: [baseball.yahoo.co.jp/hsb/teams/20279](https://baseball.yahoo.co.jp/hsb/teams/20279/top)
- 瀬戸内(広島): [baseball.yahoo.co.jp/hsb/teams/20330](https://baseball.yahoo.co.jp/hsb/teams/20330/top)
- 鳴門渦潮: [baseball.yahoo.co.jp/hsb/teams/20396](https://baseball.yahoo.co.jp/hsb/teams/20396/top)
- 英明: [baseball.yahoo.co.jp/hsb/teams/20267](https://baseball.yahoo.co.jp/hsb/teams/20267/top)
- 新田: [baseball.yahoo.co.jp/hsb/teams/20066](https://baseball.yahoo.co.jp/hsb/teams/20066/top)
- 高知中央: [baseball.yahoo.co.jp/hsb/teams/20470](https://baseball.yahoo.co.jp/hsb/teams/20470/top)（春の出場記録なし、未出場として0回扱い）
- 東海大福岡: [baseball.yahoo.co.jp/hsb/teams/20391](https://baseball.yahoo.co.jp/hsb/teams/20391/top)（夏は出場なし）
- 九州国際大付: [baseball.yahoo.co.jp/hsb/teams/20242](https://baseball.yahoo.co.jp/hsb/teams/20242/top)
- 西日本短大付: [baseball.yahoo.co.jp/hsb/teams/20042](https://baseball.yahoo.co.jp/hsb/teams/20042/top)
- 清峰: [baseball.yahoo.co.jp/hsb/teams/20103](https://baseball.yahoo.co.jp/hsb/teams/20103/top)
- 九州学院: [baseball.yahoo.co.jp/hsb/teams/20270](https://baseball.yahoo.co.jp/hsb/teams/20270/top)
- 折尾愛真: [baseball.yahoo.co.jp/hsb/teams/20409](https://baseball.yahoo.co.jp/hsb/teams/20409/top)
- 龍谷(佐賀): [baseball.yahoo.co.jp/hsb/teams/20370](https://baseball.yahoo.co.jp/hsb/teams/20370/top)
- 柳ヶ浦: [baseball.yahoo.co.jp/hsb/teams/20068](https://baseball.yahoo.co.jp/hsb/teams/20068/top)
- 興南: [baseball.yahoo.co.jp/hsb/teams/20172](https://baseball.yahoo.co.jp/hsb/teams/20172/top)
- 福岡大大濠: [baseball.yahoo.co.jp/hsb/teams/20392](https://baseball.yahoo.co.jp/hsb/teams/20392/top)
- 東筑: [baseball.yahoo.co.jp/hsb/teams/19412](https://baseball.yahoo.co.jp/hsb/teams/19412/top)
- 延岡学園: [baseball.yahoo.co.jp/hsb/teams/20126](https://baseball.yahoo.co.jp/hsb/teams/20126/top)
- 日南学園: [baseball.yahoo.co.jp/hsb/teams/20186](https://baseball.yahoo.co.jp/hsb/teams/20186/top)
- 鹿児島商業: [baseball.yahoo.co.jp/hsb_spring_local/entryteams/20166](https://baseball.yahoo.co.jp/hsb_spring_local/entryteams/20166)
- 鹿児島城西: [baseball.yahoo.co.jp/hsb/teams/20420](https://baseball.yahoo.co.jp/hsb/teams/20420/top)（夏は出場なし）
- 豊見城: [baseball.yahoo.co.jp/hsb/teams/19474](https://baseball.yahoo.co.jp/hsb/teams/19474/top)
- 佐賀西: [baseball.yahoo.co.jp/hsb/teams/19422](https://baseball.yahoo.co.jp/hsb/teams/19422/top)（春の出場記録なし、未出場として0回扱い）
- 諫早: [baseball.yahoo.co.jp/hsb/teams/19432](https://baseball.yahoo.co.jp/hsb/teams/19432/top)
- 柳井学園: [baseball.yahoo.co.jp/hsb/teams/20292](https://baseball.yahoo.co.jp/hsb/teams/20292/top)（春の出場記録なし、未出場として0回扱い）
- 熊本国府: [baseball.yahoo.co.jp/hsb/teams/22959](https://baseball.yahoo.co.jp/hsb/teams/22959/top)（夏は出場なし）
- 有明(熊本): [baseball.yahoo.co.jp/hsb/teams/22943](https://baseball.yahoo.co.jp/hsb/teams/22943/top)（春の出場記録なし、未出場として0回扱い）
- 中京(岐阜): [baseball.yahoo.co.jp/hsb/teams/20162](https://baseball.yahoo.co.jp/hsb/teams/20162/top)
- 掛川西: [baseball.yahoo.co.jp/hsb/teams/20223](https://baseball.yahoo.co.jp/hsb/teams/20223/top)
- 豊川: [baseball.yahoo.co.jp/hsb/teams/20337](https://baseball.yahoo.co.jp/hsb/teams/20337/top)（夏は出場なし）
- 至学館: [baseball.yahoo.co.jp/hsb/teams/20287](https://baseball.yahoo.co.jp/hsb/teams/20287/top)
- 誉: [baseball.yahoo.co.jp/hsb/teams/20416](https://baseball.yahoo.co.jp/hsb/teams/20416/top)（春の出場記録なし、未出場として0回扱い）
- 享栄: [baseball.yahoo.co.jp/hsb_summer_local/entryteams/19249](https://baseball.yahoo.co.jp/hsb_summer_local/entryteams/19249)
- 聖隷クリストファー: [baseball.yahoo.co.jp/hsb/teams/20503](https://baseball.yahoo.co.jp/hsb/teams/20503/top)（春の出場記録なし、未出場として0回扱い）
- 日大三島: [baseball.yahoo.co.jp/hsb/teams/19242](https://baseball.yahoo.co.jp/hsb/teams/19242/top)
- 加藤学園: [baseball.yahoo.co.jp/hsb/teams/20421](https://baseball.yahoo.co.jp/hsb/teams/20421/top)（夏は出場なし）
- 藤枝明誠: [baseball.yahoo.co.jp/hsb/teams/20400](https://baseball.yahoo.co.jp/hsb/teams/20400/top)（春の出場記録なし、未出場として0回扱い）
- 東海大静岡翔洋: [baseball.yahoo.co.jp/hsb/teams/20024](https://baseball.yahoo.co.jp/hsb/teams/20024/top)
- 岐阜第一: [baseball.yahoo.co.jp/hsb/teams/19261](https://baseball.yahoo.co.jp/hsb/teams/19261/top)
- 社: [baseball.yahoo.co.jp/hsb/teams/20479](https://baseball.yahoo.co.jp/hsb/teams/20479/top)
- 明石商: [baseball.yahoo.co.jp/hsb/teams/20378](https://baseball.yahoo.co.jp/hsb/teams/20378/top)
- 神戸国際大付: [baseball.yahoo.co.jp/hsb/teams/20059](https://baseball.yahoo.co.jp/hsb/teams/20059/top)
- 郡山(奈良): [baseball.yahoo.co.jp/hsb/teams/19087](https://baseball.yahoo.co.jp/hsb/teams/19087/top)（春の出場記録なし、未出場として0回扱い）
- 奈良大付: [baseball.yahoo.co.jp/hsb/teams/20357](https://baseball.yahoo.co.jp/hsb/teams/20357/top)
- 京都外大西: [baseball.yahoo.co.jp/hsb/teams/20028](https://baseball.yahoo.co.jp/hsb/teams/20028/top)
- 東山: [baseball.yahoo.co.jp/hsb/teams/19288](https://baseball.yahoo.co.jp/hsb/teams/19288/top)
- 花園: [baseball.yahoo.co.jp/hsb/teams/19291](https://baseball.yahoo.co.jp/hsb/teams/19291/top)
- 福知山成美: [baseball.yahoo.co.jp/hsb/teams/20142](https://baseball.yahoo.co.jp/hsb/teams/20142/top)
- 乙訓: [baseball.yahoo.co.jp/hsb/teams/20404](https://baseball.yahoo.co.jp/hsb/teams/20404/top)（夏は出場なし）

（帝京大可児は候補に挙がったが、甲子園出場が0回だったため対象外とした。）

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
