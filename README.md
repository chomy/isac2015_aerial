# isac2015_aerial
### やりたいことリスト
#### 最上位タスク
- 現在までの進捗のまとめ作業を行い、まとめwiki(仮)を作成すること
	- http://www.hi-rezclimate.org/
	
	##### まとめwiki(仮)内容は以下のモノ
	- 上記アドレス内にあるマップの作成方法のドキュメント・手順書・ソースコードの作成公開(作ったヤツがいいなら)
	- 内部閲覧用(サーバーのIP・MACなど)ハードコードの場合は台帳を作成し、ドキュメントと対応させること<font color="red">IP台帳等の攻撃対象になる恐れのあるものは、これを公開しない</font>
	- 中尾さんの私物サーバーに負荷をかけると申し訳ないので、大友のサーバーに引っ越し(当日までにサーバー立てておきます)
		- このままでもいいよ。私が都合よく遊べるから。（なかお）
		- どっかから(いくつかある)サーバーの金券をもらう。
		- 別に立てる場合も、Debianで....100歩譲ってUbuntuで....
	- リンク切れ等の確認・修正作業 （これは中尾がやります）
		- 現在データのバージョンアップ中で、データが更新されてません。
		- APIリクエストのJSONが止まっていること
		- マップの一部が更新が止まっていること


#### 個人的にやりたいことは、遠慮なく追記してください

- arduinoかなんかの基盤にセンサーつけて、ロガーを作ること
	- Wifiが載っていることを考えると、Edisonが良いかも。
	- まぁこれは作れます。
- 作ったロガーの取得データをMAP上に反映させること
	- デバイスが作れれば、これも可能
- 過去数日分のデータから安全なルートか、安全ではないルートかの(判断はしない)ゆるい描画
- 海浜公園のデータ整形と気象データの相関関係探る
- 去年のAPI進化させるのどうじゃろ??JAXAのデータは立場的に公開できない(科学的に精緻なことを条件に)一部切り落としたL3を、ラグランジュかなんか(単純に移動平均でもいい)で「補完」して陸域と海域の境界ギリギリとかまでAPIアクセスできるしh5に戻してGCOMToolsとかで描画する??
	- 職業上、私もJAXAと同じサイドにいるので、これはちょっと....
- 役所だとできない、役所だから出来ないことやりたい。(国交省と海保とJAXAのデータで地球観測・マッピング)
	- であれば、国交省から河川とダムの水位データを、JAXAのGSMaP/GCOM-W1 etc.から降水量その他をもらってきてマッピングすれば、国内に限られるけどOfficial Challenge のClean Water Mappingにapplyできる。
	- 世界に関しては、OSMの井戸、水道のタグが付いた位置をマッピング。
	- あと、だいちが水域のデータを観測していないかなぁ
	- 水質センサが作れれば、それをバラまいて....
	- 湯村さんはOfficial Challengeにこだわっている気がするので、こじつけでもOfficial Challenge に絡めておいたほうが良い気がする....

#### ISAC2015 Official Challenge でできそうなことを列挙してみる

なんかアイデアソンがOfficial Challenge 前提だったっぽいので。
- Open-Source air traffic tracking
	- まぁぶっちゃけ航空機の位置をマッピングするくらいなら、すぐできる。
	- Flightrader24のデータサイトもハッキング済w
	- NASAから、ハッカソンで使うデータが公開されている。
	- backendでフライトシミュレータ動かして...みたいな課題もできそうっちゃぁできそう
- Clean Water Mapping
	- OSMの井戸、水道、などのタグが付いた位置をマッピングするとか。
	- しずくの降水量、積雪深はそのまま使える。
	- https://2015.spaceappschallenge.org/challenge/clean-water-mapping/
- Crop Alert
	- サービスだけなら作れそう。
	- アイデアソンでチーム作っている人がいるっぽい
	- すでに大平さんが....
	- https://2015.spaceappschallenge.org/challenge/crop-alert-learning-growers/

我々にとってチャレンジになるのは、Open-Source air traffic tracking かな。まぁトラフィックデータのライセンスは真っ黒だけどw
- https://www.marinetraffic.com/jp/ これがセーフならセーフでしょwww
