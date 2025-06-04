# 課題
# GitHubまとめ

GitHubのダウンロードと使い方

FlutterはGoogleの作ったモバイルアプリ開発用のUIフレームワーク

AndroidとiOSアプリ開発において開発効率を向上させたい場合に有効なフレームワーク

Web・デスクトップアプリケーションのサポートもされるようになった

# 使用言語

Flutterはdartという言語を使う

mainメソッドは

void main() {

}

プリントは

print("Hello!!");

文法や使用感はJavaに近く、オブジェクト指向の言語

# まとめ

FlutterはGoogleの作ったフレームワーク

Dartという言語を使い、オブジェクト指向の言語

2025/05/27

# 教科書3-3

レイアウトのソースからボタン配置などをやりました。

アラートやダイヤルログを中心にやりました。

# showDialog関数について

showDialog(
  context: <BuildContext>
  builder: <WidgetBuilder>
)

contextはBuildContextインスタンスを指定し、context上にダイアログが表示される

builderはWidgetBuilderは、表示するウェジットにを生成する関数

# AlertDialogについて

AlertDialog(
  title: ウェジット
  content: ウェジット
)

タイトルとコンテンツとしてウェジットををshowDialogで表示させる

# アラートにボタンを追加する

action: <Widget> [
  ウェジットのリスト
]

showDialog(...).then<void>(...処理...)

# SimpleDialogについて

SimpleDialog(
  title: ウェジット
  children: [ウェジットのリスト]
)

# SimpleDialogOptionについて

SimpleDialogOption(
  child: ウェジット
  onPressed: ...処理...
)

2025/06/03

# 4-1教科書

AppBarについて

AppBar(
  title: ウェジット,
  leading: ウェジット,
  actions: <Widget>[ウェジットのリスト],
  bottom: <PreferredSize>,
)

AppBarにウェジットとプロパティ、４つのエリアに配置できる

# actionについて

actions: <Widget>[
  IconButton(
    icon: Icon(Icons.android),
    tooltip: 'add star...',
    onPressed: iconPressedA,
  )
]

IconButtonのインスタンスを用意
actionはタイトルの右側に表示されるので、アイコンなどの小さいスペースが表示内容がわかるものを使う

# 4-2 

# ナビゲーターについて

Navigatorクラスというクラスが用意されてる
画面切り替えなどをする

移動先をプッシュする
Navigator.push(<BuildContext>,<Route>);

移動をポップする
Navigator.pop(<BuildContext>);

2025/06/04