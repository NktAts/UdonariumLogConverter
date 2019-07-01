# Udon傍（うどんそば） -- ユドナリウムのログコンバータ

![うどんそば](assets/icon/うどんそば.png "うどんそばアイコン")

製作者：りょーさん

## 更新履歴

* 2019/7/1：Ver1.0、テキストファイルを読み、タブごとに出力する機能を追加
* 2019/6/26：Ver0.2、Githubに登録。READMEを.mdファイルに変更
* 2019/6/25：Ver0.1、初期作成  

## 概要
ユドナリウムのルームデータから、参照に適したHTMLファイルを生成するバッチファイルです。  

## 動作確認環境
製作者は以下の環境にて動作確認を行っています。  
以下の環境以外での動作は保証いたしません。  

* OS:Windows10 64bit  
* ブラウザ：Google Chrome  
* ユドナリウム：Ver1.9.2によって作成されたルームデータ  

## 使用方法
1. 「input」フォルダに、ルームデータのzipファイルを1つだけ格納してください。
1. 「input」フォルダに入っている「chat-tab.txt」に、出力したいタブのタブ名を1行ごとに記載してください。
1. 「udon_soba.bat」をダブルクリックして実行してください。
1. コマンドプロンプトが開き、「続行するには何かキーを押してください . . .」と出力されたらキーを押してください。
1. 実行したフォルダに「output_(日時)」というフォルダができていると思うので、フォルダごと好きな場所に移動してください。  ※フォルダ名や、中のHTMLのファイル名を変更しても問題なく閲覧可能です。

## 内容物
* assetsフォルダ

必要なツール、画像、XSLTファイルなどが格納されています。追加・削除・変更を行わないでください。

* inputフォルダ

このフォルダに、生成したいログが入ったルームデータをzipごと格納してください。

* temporaryフォルダ

ルームデータの一時展開用フォルダです。この中にフォルダやファイルを入れないでください。

* output_(日時)フォルダ

実行後に生成されるHTMLファイルと画像フォルダです。
「converted_chatlog.html」にはすべてのチャットを時刻でソートしたものが、
「converted_chatlog_(タブ名).html」には指定したタブのみのチャットが出力されます。

* udon_soba.bat

生成プログラム本体です。内容の変更を行わないでください。

* README.md

Githubで表示するときのREADMEです。

* README.html

このファイルです。

## 使用上の注意
* 例外処理がとても雑です。  ルームデータ以外を格納する、処理途中で中断して再実行するなどを行った場合に想定しない動作をする場合があります。  自力での対処が難しい方は、使用方法を守り、フォルダ構成がおかしくなったら元のコンバータを再取得してください。

## 現時点で気づいている不具合や仕様
* ダイスボットは、初期画像(黒い人型)で表示されます。

* トランプやダイスをキャラクターやプレイヤーの画像として使用した場合、画像が表示されません。

## 行いたい改修項目

* CSS対応
* スマホも想定したデフォルトCSSの作成
* ダイスボット使用時のアイコンをダイスに変更
* トランプ・ダイスを使用したときの画像対応
* 日時のHH:MM:SS表示
* Typescript+HTML+CC形式にしてどこかのサイトで公開

## 使用しているソフトウェア
以下のソフトウェアを使用しています。

* 7-Zip(https://sevenzip.osdn.jp/)
* msxsl.exe(https://www.microsoft.com/en-us/download/details.aspx?id=21714)

## 使用している素材
ユドナリウムと同様に、以下を素材として使用しています。

* ©無料素材倶楽部 (http://sozai.7gates.net/)
* ©Ｒド (http://www.geocities.co.jp/Milano-Cat/3319/)
* ©きまぐれアフター (http://www5d.biglobe.ne.jp/~gakai/)
* ©鍛冶屋黒胡椒 (https://www15.atwiki.jp/smith_blp/pages/1.html)
* ©Material.io (https://material.io/tools/icons/)


## おまけ
* 使用した際に、製作者のTwitter(@NktAts)に連絡をくれるととても喜びます。

* 少し詳しい人が見れば、各所に豪快な仕様が見られると思います。（画像の扱いとか）  全ては製作者の技術力が拙いためです。誰か助けてください。


## 連絡先  
お問い合わせ・要望・不具合報告・改善アドバイス・感想などは、以下のいずれかの手段でご連絡ください。

* 製作者のTwitterアカウント(@NktAts)にリプライやDM
* Github(https://github.com/NktAts/UdonariumLogConverter)にissueとして投稿


(以上)