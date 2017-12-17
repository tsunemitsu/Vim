# Vim

### モード
- ノーマルモード
- 入力モード (i)
- コマンドモード (:)
- ビジュアルモード (v)

### ファイルの保存/読み込み
|コマンド|説明|
|:--|:--|
|:w|保存|
|:w file名|名前をつけて保存|
|:wq|保存して終了|
|:q|終了|
|:q!|強制終了|
|:e file名|ファイルを開く|

### 移動系
|コマンド|説明|
|:--|:--|
|j|上|
|k|下|
|h|左|
|l|右|
|gg|ファイルの先頭へ移動|
|G|ファイルの末尾へ移動|
|Ctrl + b|画面の一番上へ移動|
|Ctrl + f|画面の一番下へ移動|
|w|次の単語へ移動|
|e|次の単語の終わりへ移動|
|b|前の単語へ移動|
|^|行頭へ移動|
|$|行末へ移動|
|f + char|charへ移動|
|;|次のcharへ移動|
|%|カッコの上で押すと対応するカッコへ移動|

### 選択系(ビジュアルモード)
|コマンド|説明|
|:--|:--|
|V|行を選択|
|Ctrl + v|矩形選択|
|gg + V + G|全選択|

### カット(削除)、コピー、貼り付け
|コマンド|説明|
|:--|:--|
|x|一文字削除(カット)|
|dd|行削除|
|数字 + dd|数字分行を削除|
|p|貼り付け|
|yy|コピー|
|数字 + yy|数字分行をコピー|

### 検索、置換
|コマンド|説明|
|:--|:--|
|/ + char|charを検索|
|n|次を検索(下)|
|N|次を検索(上)|
|*|カーソルがある位置の文字を検索(下)|
|#|カーソルがある位置の文字を検索(上)|
|:s/置換前/置換後|行を対象に一致した最初のものを置換|
|:s/置換前/置換後/g|行を対象に一致した全てを置換|
|:%s/置換前/置換後/g|ファイルを対象に一致した全てを置換|
|:%s/置換前/置換後/gc|ファイルを対象に一致した全てを置換(置換前に1つ1つ確認する)|

### 操作の取消、繰り返し
|コマンド|説明|
|:--|:--|
|u|元に戻す(undo)|
|Ctrl + r|undoした操作を元に戻す|
|.|前の操作を繰り返す|

### ウィンドウ、タブ
|コマンド|説明|
|:--|:--|
|:sp|ウィンドウを上下に分割|
|:vs|ウィンドウを左右に分割|
|Ctrl + w|ウィンドウを移動する|
|:close|ウィンドウを閉じる|
|:tabnew|新規タブを開く|
|gt|タブを移動する|
|:tabclose|タブを閉じる|
|vim -p file1 file2|複数fileを複数タブで開く|
|tabdo :s/〜|全てのタブを対象に置換する|


### その他
|コマンド|説明|
|:--|:--|
|=|インデントを揃える|
|Ctrl + n|入力補完|
|:set number|行番号を表示|
|:set nonumber|行番号を非表示|
|:syntax on|文書を色付け|
|:syntax off|文書の色付けを消す|





|コマンド|説明|
|:--|:--|
|||
|||
|||
|||
|||
|||
|||





