# erabasic サクラエディタ用設定ファイル

## 動作確認環境

OS `Windows 10 Pro 64bit`  
サクラエディタ `Ver.2.3.1.0`  
正規表現ライブラリ `bregonig.dll Ver.4.11 with Onigmo 6.1.1`  

正規表現ライブラリが入ってない方は
[正規表現ライブラリ bregonig.dll](http://k-takata.o.oo7.jp/mysoft/bregonig.html) から
ダウンロードしてください。

## 使い方

サクラエディタを起動して、下記の手順でセットアップ。

1.`［設定］`→`［共通設定］`  
![［共通設定］を選択](https://github.com/E2-ETSU/erabasic/wiki/image/sakura_kyoutsuu.png)


2.左下の`［設定フォルダ］`→`［開く］`  
![［設定フォルダ］を開く](https://github.com/E2-ETSU/erabasic/wiki/image/sakura_hiraku.png)

3.表示されたフォルダに設定ファイル群を丸ごとコピーする。

4.`［設定］`→`［タイプ別設定一覧］`を開く。  
![［タイプ別選択一覧］を選択](https://github.com/E2-ETSU/erabasic/wiki/image/sakura_type_betsu.png)

5.一番下の設定（例では設定ファイル）を選択してから`［インポート］`を選択する。  
![インポート時は一番下を選択する](https://github.com/E2-ETSU/erabasic/wiki/image/sakura_import.png)

6.`［EraBasic.iniを指定］`→`［新規追加/そのままインポート］`  
![［タイプ別選択一覧］を選択](https://github.com/E2-ETSU/erabasic/wiki/image/sakura_import_ok.png)

7.`定義確認用ソースファイル.ERB`をサクラエディタで開く。

8.もう一度`[タイプ別設定]`を開き、追加された`erabasic`を`［一時適用］`する。

9.これで色分け設定が有効になります。  
![［タイプ別選択一覧］を選択](https://github.com/E2-ETSU/erabasic/wiki/image/sakura_erb_example.png)

## ファイル群についての説明

+ `EraBasic.ini`  
   _サクラエディタのタイプ別設定_ のインポートファイル
+ `ERB.rkw`  
   _正規表現キーワード_ のインポート用ファイル
+ `ERB_COMMAND.kwd`  
   _強調キーワード1_ 命令・式中関数
+ `ERB_CONTROL.kwd`  
   _強調キーワード2_ IFやFOR、REPEATなどの制御構文
+ `ERB_RESERVED.kwd`  
   _強調キーワード3_ #DIMなどの予約語
+ `ERB_VAR_NUM.kwd`  
   _強調キーワード4_ CFLAGなどの数値型変数
+ `ERB_VAR_STR.kwd`  
   _強調キーワード5_ CALLNAMEなどの文字列型変数
+ `ERB_DEBUG.kwd`  
   _強調キーワード6_ ASSERTなどのデバッグモード時のみ有効な命令（変数は除く）
+ `定義確認用ソースファイル.ERB`  
   色分け確認用のerabasicコード。eramaker/Emueraでは読ませないでください  
