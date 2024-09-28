# Dockerfile脆弱性診断ツール：DoChecker
DoCheckerはDockerfileの脆弱性を調査するVisual Studio Code（VSCode）の拡張機能です．
DoCheckerの動作のイメージ図は以下のものとなっています．
![画像1](https://github.com/user-attachments/assets/4bcd1da8-b484-43b7-9d9e-cd4b730f0d73)

Dockerfileに記載したパッケージの情報（パッケージ名、バージョン情報）をもとに、NISTが提供するCVE APIと照合し、記載したパッケージが持つ可能性がある脆弱性について、診断・警告します．

## インストール方法
始めに示したように、DoCheckerはVSCodeの拡張機能となっている．
このため，VSCodeの拡張機能導入方法についてはMicrosoftが提供するページを参照してほしい．
URL：https://learn.microsoft.com/ja-jp/power-pages/configure/vs-code-extension

DoCheckerに関するファイルは、本ページのDoChecker.vsixを配置しているため、これをVSCodeの拡張機能としてインストールする．
具体的なインストール手順を以下に示す．
---
(1) VSCodeの拡張機能画面を開く．
![スクリーンショット 2024-09-28 144814](https://github.com/user-attachments/assets/cbe46821-f5b3-4861-989c-5ad9c18ad62f)


(2) VSCodeの拡張機能画面の右上の「・・・」をクリックし，「VSIXからインストール」を選択．
![スクリーンショット 2024-09-28 144838](https://github.com/user-attachments/assets/2ea17431-6a94-4f11-831f-c026e75ebcad)


(3) DoChecker.vsixを選択．
＜図＞

---

これにより，DoCheckerを利用可能となる．

## DoCheckerの使い方
DoCheckerでは、NISTが提供するCVE APIを利用するため、オフライン上で利用できない点については注意してください．

DoCheckerをインストールできた方は、VSCode上でDockerfileを開いてみてください．
DoCheckerはVSCode上のDockerfileがアクティブエディタとなったとき，もしくは保存されたときに脆弱性診断を行います．
DoCheckerが正常に動作している場合は以下のような出力が得られると思います．

![スクリーンショット (5)](https://github.com/user-attachments/assets/e689498b-4557-442c-9786-01368840652c)


## 開発者
セキュリティ讃歌

## 開発に貢献する方法

## ライセンス
