### ひな形 コピー＆ペーストして, 使用して下さい。
## ↓
***
* 追加内容
	-

* bugfix
	-

* 参考サイト
	- [Markdown 記法 サンプル集](http://qiita.com/tbpgr/items/989c6badefff69377da7)

#### 記述者 : 氏名, 記述日 : 年月日 日時
***
***
### 過去のChangelog.mdファイルは, Archive01_Changelog.md,
* __Archive02_Changelog.md__
### として, ルート直下に置いてありますので, 併せて確認下さい。
### ファイル容量が20KBに達したら, 連番でArchiveしていきます。
### 最新のログは, Changelog.mdとします。
***
***
***
***
* 追加内容
	- スタートシーン ( タイトルシーン ), ゲームオーバーシーン, ポーズシーン, リ
		トライ機能の追加。
	- ThiredPersonCharacter の移動制限処理, Help アイコンに近づくとエンドー
		シーンに切り替わる処理。
	- レベルブループリントと BP_Widget ブループリントを主にいじりました。コメン
		ト文を付してあるので確認宜しくお願いします┌┤´д`├┐。
	- エンドシーンなどの画像を前プロジェクトからインポートしました。
		Texture フォルダに格納されています。

* 既知のバグ
	- ゲームをプレイする時々によって, カメラの向く方向が違う事象。
	- C キーでのカメラ視点切り替えがおかしくなるときがある事象。
	- ゲームプレイをした時に, キャラクターを高台から落ちずキャラクターが同じ高さ
		で移動してしまう事象。
	- タイトルシーンやエンドシーンなどの内部ロジックは, まだまだ改善の余地ありな
		ので自分が納得できる様な処理を追加してもらえると助かります。

#### 記述者 : 牛山 拓成, 記述日 : 2017年01月01日(日) 午前2時28分
***
* 追加内容
	- Material'/Game/Geometry/Materials/' に, 赤・緑・青のマテリアルを作成
		し, 追加しました。
	- StaticMesh'/Game/Geometry/Meshes/SM_ItemTestMesh.SM_ItemTestMesh'
	を作成し, 追加しました。 レベル上に置いてある丸形の Mesh です。
	- WidgetBlueprint'/Game/BP/BP_Widget.BP_Widget' の処理にアイテム表示
		処理を追加しました。
	- レベルブループリントにアイテム表示処理を追加しました。

* bugfix
	- なし。

* 参考サイト
	- [StaticMesh への色つけ参考サイト](http://colorcube.jugem.cc/?eid=223)
	- [UE4 での命名規則参考サイト](https://wiki.unrealengine.com/Assets_Naming_Convention_JP)
	- [配列ノード | Unreal Engine](https://docs.unrealengine.com/latest/JPN/Engine/Blueprints/UserGuide/Arrays/ArrayNodes/index.html)

#### 記述者 : 牛山 拓成, 記述日 : 2017年01月11日(水) 午前9時02分
