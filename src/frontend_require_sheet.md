# 静的サイト構築におけるフロントエンド実装スキル要件シート
> ○ → 必須選択（基本一つのみ）  
> □ → 任意選択（複数可）  
> 備考には記載のないツール名、versionなどを入力すると良いかもしれません

## htmlの作成・出力方法
|選択|要件|備考|
|:--|:--|:--|
|○|特になし|コンパイル後ファイルだけで、管理上問題が無ければこれを選ぶ|
|○|テンプレートエンジン|例: jade|
|○|静的サイトジェネレータ|例: Jekyll|
|○|その他||
|□|元データを納品物に含める（コンパイルする場合）||

## ファイルの共通化（インクルード）
|選択|要件|備考|
|:--|:--|:--|
|○|しない||
|○|SSI||
|○|PHP|.html内でphpを使用|
|○|DreamWeaverのテンプレート||
|○|JavaScriptで読み込む||
|○|テンプレートエンジン||
|○|静的サイトジェネレータ||
|○|その他||
|□|元データを納品物に含める（コンパイルする場合）||
※どこまでファイルを細分化するかは要検討
※表示ページごとに多少の差異がある場合、施策を要検討

## タスクランナー
|選択|要件|備考|
|:--|:--|:--|
|○|使わない|コンパイル後ファイルだけで、管理上問題が無ければこれを選ぶ|
|○|Gulp||
|○|Grunt||
|○|その他||
|□|設定ファイルにaltJSを使用する||
|□|設定ファイルを納品物に含める|gulp.jsやpackage.jsonなど|

----

## cssプリプロセッサ
|選択|要件|備考|
|:--|:--|:--|
|○|使わない||
|○|sass||
|○|scss||
|□|compassを使用||
|○|less||
|○|その他メタ言語|例: stylus|
|□|cssを圧縮する||
|□|タスクランナーを使用||
|□|コマンドラインを使用||
|□|その他ツールを使用||
|□|元データ・設定ファイルを納品物に含める||

## cssスプライト
|選択|要件|備考|
|:--|:--|:--|
|○|しない||
|○|手作業で対応||
|○|プリプロセッサを使用||
|○|タスクランナーを使用||
|○|その他|例: python, glue|

## cssフレームワーク
|選択|要件|備考|
|:--|:--|:--|
|○|使わない||
|○|Bootstrap||
|○|Foundation||
|○|Gumby||
|○|その他||
|□|フレームワークを改造して使用する（class名など）||

----

## JSライブラリ
|選択|要件|備考|
|:--|:--|:--|
|○|使わない||
|○|以下いずれかを使用||
|□|jQuery1.X||
|□|jQuery2.X||
|□|Zepto||
|□|Prototype||
|□|jQuery Mobile||
|□|Modernizr||
|□|Underscore||
|□|CreateJS||
|□|レガシーブラウザ対策|例: IE9.js, html5shiv.js|
|□|その他||

## JSの結合
|選択|要件|備考|
|:--|:--|:--|
|○|しない||
|○|タスクランナーを使用||
|○|その他||
|□|元データを納品物に含める||

## JSの圧縮
|選択|要件|備考|
|:--|:--|:--|
|○|しない||
|○|タスクランナーを使用||
|○|その他||
|□|元データを納品物に含める||

----

## altJS
|選択|要件|備考|
|:--|:--|:--|
|○|使わない||
|○|CoffeeScript||
|○|TypeScript||
|○|Haxe||
|○|その他||
|□|元データを納品物に含める||

## png画像の最適化
|選択|要件|備考|
|:--|:--|:--|
|○|しない||
|○|タスクランナーを使用||
|○|その他|例: PNGGauntletを使用|

## Webフォント（アイコンフォント）
|選択|要件|備考|
|:--|:--|:--|
|○|使わない||
|○|以下いずれかを使用||
|□|Google Web Fonts||
|□|Typekit||
|□|Fonts.com||
|□|Font Awesome||
|□|その他|独自のフォント含む|
|□|class名を変更して使用する||