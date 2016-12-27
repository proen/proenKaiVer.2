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
### 過去のChangelog.mdファイルは, Archive01_Changelog.md
### として, ルート直下に置いてありますので, 併せて確認下さい。
### ファイル容量が20KBに達したら, 連番でArchiveしていきます。
### 最新のログは, Changelog.mdとします。
***
***
***
***
* 追加内容
	- ブロック　白_改 キューブをレベル上に置いて, ビルドすると,
        黒く焼けてしまう事象を, DirectionalLight の詳細タブにある
        Light→シャドウを落とすのチェックを外し解決した。
    - ThirdPersonブループリント→Tutorial02_2DMapの読み込みとunload処理
        →処理内容コメントの追加＆Tutorial02_2DMapのロード・アンロード処理に変更した。
        ロード・アンロード処理の境界線を調整した。
    - ThirdPersonブループリント→Tutorial03_2DMapの読み込みとunload処理
        →Tutorial03_2DMapのロード・アンロード処理に追加した。

* bugfix
	- とくになし。

* 参考サイト
	- [Markdown 記法 サンプル集](http://qiita.com/tbpgr/items/989c6badefff69377da7)
    - [アンリアル エディタでファイルをチェックアウトする(GIT HUB)](https://docs.unrealengine.com/latest/JPN/Engine/Basics/SourceControl/InEditor/index.html)
    - [warning: refname 'HEAD' is ambiguous(GIT HUB)](https://gotohayato.com/content/11)

#### 記述者 : 牛山 拓成, 記述日 : 2016年08月01日(月) 午前2時04分
***
* 追加内容
	- TestStage系統マップで制作したマップを間違って編集し, 壊さないために, 編集できないようにロックを掛けました。
    - 平田が制作した, チュートリアル 3DMAP を基に, Tutorial01_3DMap, Tutorial02_3DMap, Tutorial03_3DMap
        に牛山がそれぞれ分けて格納しました。制作したマップに不備があったので一部, 修正を行いました。
    - ThirdPersonブループリント→レベル起動時に, 2Dから3Dに切り替えたときに, 2DMAPが消え, Yを真ん中の座標にし, 落ちるのを防いでいる処理
        を追加しました。
    - ThirdPersonブループリント→レベル入れ替え&3D座標位置維持
        に Tutorial01 ～ 03 までの 2DMAP のアンロード処理を追加しました。
    - ThirdPersonブループリント→2DMAP時のレベル変更処理
        で Tutorial01_2DMap をロード, Tutorial01_3DMap をアンロードする処理を追加しました。
    - チュートリアルマップの 3D の 1 ～ 3 マップで, レベルのロード・アンロード処理を追加しました。
        ここまでの, 作業により, チュートリアルマップ 2D, 3D 全体で, 動作するようになりました。
    - パーシスタントレベルに, ブロックの表示・非表示処理を追加しました。
    - Mesh フォルダにやすさんから, maya で作成した, Materialを多数追加しました。
        Mesh などに色を適用したい場合は, このフォルダを使うと良いかもしれません。
    - __今回, 追加した機能が多いので, 書き切れてない部分があります。
        競合が発生した場合は, Unreal Engine の DIFF の機能を試して見て下さい。__


* bugfix
	- _Tutorial03_3DMap の特定箇所で, カメラ切り替えすると, Player が, アクターにハマってしまう
        事象が確認されたため, BoxTrigger を 2 カ所に配置しました。
        まだ, Trigger 処理 を書いていないので, 次回は, ここから対処していく。_

* 参考サイト
	- [Statick Mesh の表示・非表示処理の仕方参考サイト](https://answers.unrealengine.com/questions/262267/set-visibility-set-actor-hidden-in-game-switches-f.html)

#### 記述者 : 牛山 拓成, 記述日 : 2016年08月02日(火) 午後4時56分
***
* 追加内容
	- 「Tutorial03_2DMap, Tutorial02_3DMap, Tutorial03_3DMap」のレベルブループリントに,
        カメラの切り替えが出来る地点, カメラの切り替えが出来ない地点 を追加した。また, これらのレベル
        に, トリガーボックスを幾つかの地点に配置しました。
    - 現時点でのマップ構成での, Characterが, Map上で, カメラの切り替えをすると, 不整合を起こす事象を全て改善しました。

* bugfix
	- _「Tutorial03_3DMap の特定箇所で, カメラ切り替えすると, Player が, アクターにハマってしまう
        事象が確認されたため, BoxTrigger を 2 カ所に配置しました。
        まだ, Trigger 処理 を書いていないので, 次回は, ここから対処していく。」_ __解決しました。___

* 参考サイト
	- とくになし。

#### 記述者 : 牛山 拓成, 記述日 : 2016年08月11日(木) 午後6時16分
***
* 追加内容
	- __Changelog.md__ と __README.md__ の誤字＆脱字を修正しました。詳しい修正箇所は
		, 変更履歴を見てください。

* bugfix
	- とくになし。

* 参考サイト
	- とくになし。

#### 記述者 : 牛山 拓成, 記述日 : 2016年08月16日(火) 午前0時55分
***
* 追加内容
	- Character の移動速度が遅いという指摘を受けたので, 移動速度を少し速くしました。
        character movement 項目内
        max walk speed : 124.0 → 200.0
    - １日の, 朝・昼・夜の表現処理の追加を行いました。
        TestStage レベルブループリント内に, sunSpeed という変数が存在するので
        ここで, 太陽の傾き速度の調整が行えるようになっています。
        実装方法にいては, YouTube にある, TimeOfDay という, 動画を参考にして実装を行いました。
	- Changelog.md の脱字＆誤字を修正しました。

* bugfix
	- 特になし。

* 参考サイト
	- [answer hub 質問項目](https://answers.unrealengine.com/questions/500459/%E3%82%AB%E3%83%A1%E3%83%A9%E3%81%AE%E8%A6%96%E7%82%B9%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6.html)
    - [日の傾き解説サイト](https://www.youtube.com/watch?v=xt_TIYthRUE)

#### 記述者 : 牛山 拓成, 記述日 : 2016年10月04日(火) 午後4時50分
***
* 追加内容
	- ThirdPersonブループリント内に GameOverTime 変数を追加しました。
		この変数は, ゲームのゲームオーバータイムの時間を設定する変数です。
		ここでは, 5 分に設定しました。
	- Git_Proen\Content\DATA\contents_examples_help_icon.t3d
		を追加しました。くるくる回る HELP ICON です。
		UE4 の機能別サンプルから, エクスポートした後, 当該プロジェクト
		で, インポートしました。ライセンスは, UE4 で作ったゲームに限られています。
	- ThirdPersonブループリント内に, Eキーでの, 看板へのズーム機能
		非ズーム機能, 表示＆非表示処理を追加しました。
	- ThirdPersonブループリント内のキャラクター＆カメラの配置位置のメモです。
		SpringArmコンポーネント内内包
	- ForwardCamera {
			location : 213, 0, 155,
			rotation : 0, -30, 180,
			zoom : 1, 1, 1
		}
	- BackCamera {
			location : -203, 0, 155,
			rotation : 0, -30, 0,
			zoom : 1, 1, 1
		}
	- 2DCamera {
			location : 1, 1000, -45,
			rotation : -0, -0, -90,
			zoom : 1, 1, 1
		}
	- Character {
			location : 0, 0, -100,
			rotation : 0, 0, -90,
			zoom : 1, 1, 1
		}

* bugfix
	- 特になし。

* 参考サイト
	- 特になし。

* 次回, 実装したい機能
	- カメラが壁にめり込まない処理。

#### 記述者 : 牛山 拓成, 記述日 : 2016年11月01日(火) 午後4時30分
***
* 追加内容
	- Tutorial03_3DMap の奥から縦 2 列に, キャラクターのカメラの
		深度によって透明度が変わる Material を適用しました。
	- Material/Transparency_Material の Material 処理を一部変更しました。
	- 透明マテリアルの基本色を白色に変更しました。
	- ThirdPerson Character の前カメラと後ろカメラをキャラクターに近づけ
		ました。( 透明処理で見づらかったため )
	- ヤスさんが, 作成した, ブタと羊をインポートし, TestStage 上に置きまし
		た。( StaticMesh'/Game/Character/羊.羊',
		StaticMesh'/Game/Character/ぶたさん.ぶたさん' )

* bugfix
	- 透過処理のマテリアルを適用した actor の色が適用されない！？←
		改善する必要がある。

* 参考サイト
	- [Unreal Engine | マテリアル エディタ - 透過処理の操作ガイド](https://docs.unrealengine.com/latest/JPN/Engine/Rendering/Materials/HowTo/Transparency/index.html)
	- [UE4でカメラがキャラクターに近付き過ぎたら半透明にする - ほげたつブログ](http://hogetatu.hatenablog.com/entry/2015/10/15/225613)

#### 記述者 : 牛山 拓成, 記述日 : 2016年11月15日(火) 午後4時28分
***
* 追加内容
	- Content\DATA\Backup\制限時間.png 制限時間スクリプトのバックアップ
	- SandBoxie.uproject : 「"Enabled": true」→「"Enabled": false」に
		変更を行いました。(LowEntryExtendedStandardLibraryが無効になった
		ので再度有効にする際には, Enabled": true にして下さい。)
	- Widget ポーズ画面の表示＆非表示処理から行っていく。
		(2016年12月06日(火	)12時49分完了)
	- ポーズ画面にしたときに、Playしていた画面を背景にしました。
		__画面を薄暗くする処理を実装していく。__
	- ThirdPersonブループリント内のゲームオーバー画面処理を
		ポーズ画面処理に変更しました。
	- ThirdPersonブループリント内, スタート画面時の
		キー処理の処理を大幅に変更しました。

* bug
	- __3D画面から2D画面に戻るときにステージが消えるバグがあります。__

* 参考サイト
	- [Markdown 記法 サンプル集](http://qiita.com/tbpgr/items/989c6badefff69377da7)

#### 記述者 : 氏名, 記述日 : 2016年12月20日(火) 午後4時40分
---
# 新プロジェクトに移行するため Archive する。
---
