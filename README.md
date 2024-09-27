# Dockerfile脆弱性診断ツール：DoChecker
DoCheckerはDockerfileの脆弱性を調査するVisual Studio Code（VSCode）の拡張機能です．
DoCheckerの動作のイメージ図は以下のものとなっています．
![画像1](https://github.com/user-attachments/assets/4bcd1da8-b484-43b7-9d9e-cd4b730f0d73)

Dockerfileに記載したパッケージの情報（パッケージ名、バージョン情報）をもとに、NISTが提供するCVE APIと照合し、記載したパッケージが持つ可能性がある脆弱性について、診断・警告します．

## インストール方法
始めに示したように、DoCheckerはVSCodeの拡張機能となっている．
このため，VSCodeの拡張機能導入方法についてはMicrosoftが提供するページを参照してほしい．
URL：https://learn.microsoft.com/ja-jp/power-pages/configure/vs-code-extension

拡張機能検索欄にDoCheckerと入力すると、候補としてDoCheckerが出てくるため、これをインストールしてください．
＜図＞

## DoCheckerの使い方
DoCheckerでは、NISTが提供するCVE APIを利用するため、オフライン上で利用できない点については注意してください．

DoCheckerをインストールできた方は、VSCode上でDockerfileを開いてみてください．
DoCheckerはVSCode上のDockerfileがアクティブエディタとなったとき，もしくは保存されたときに脆弱性診断を行います．
DoCheckerが正常に動作している場合は以下のような出力が得られると思います．

＜図＞

## 開発者
セキュリティ讃歌

## 開発に貢献する方法

## ライセンス
