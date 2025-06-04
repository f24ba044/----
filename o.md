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