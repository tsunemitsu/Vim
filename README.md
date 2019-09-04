# Vim

### 入力モードあれこれ
|コマンド|説明|
|:--|:--|
|i|通常の入力モード|
|:|コマンドモード|
|v|ビジュアルモード|
|a|カーソルの次の位置から|
|r|置換モード|
|o|行を一行追加|
|I|行頭から入力|
|A|行末から入力|
|O|前の行から入力|


### ファイルの保存/読み込み
|コマンド|説明|
|:--|:--|
|:w|保存|
|:w file名|名前をつけて保存|
|:wq|保存して終了|
|ZZ|保存して終了|
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
|<数字>G|数字で指定した行へ移動|
|Ctrl + b|画面の一番上へ移動|
|Ctrl + f|画面の一番下へ移動|
|w|次の単語の先頭へ移動|
|e|次の単語の終わりへ移動|
|b|前の単語の先頭へ移動|
|^|行頭へ移動|
|$|行末へ移動|
|f + char|charへ移動|
|;|次のcharへ移動|
|%|カッコの上で押すと対応するカッコへ移動|
|B |前の単語の先頭へ移動|

### 移動系補足：bとBの違いついて
違いは次のような単語を一語とみるかどうか
abc.def.ghi
小文字なら5単語 abc . def . ghi
大文字なら1単語 abc.def.ghi

### 選択系(ビジュアルモード)
|コマンド|説明|
|:--|:--|
|V|行を選択|
|Ctrl + v|矩形選択|
|Ctrl + v → I(Shift + i) → Ctrl + [|矩形選択した箇所に文字を入力し選択モード戻す|
|gg + V + G|全選択|

### カット(削除)、コピー、貼り付け
|コマンド|説明|
|:--|:--|
|x|一文字削除(カット)|
|dd|行削除|
|d^|カーソル位置から行頭まで削除|
|d$|カーソル位置から行末まで削除|
|D|カーソル位置から行末まで削除|
|数字 + dd|数字分行を削除|
|yy|コピー|
|p|貼り付け(カーソルの後ろ)|
|数字 + yy|数字分行をコピー|

### 検索、置換
|コマンド|説明|
|:--|:--|
|/ + char|charを下に検索|
|? + char|charを上に検索|
|n|次を検索(下)|
|N|次を検索(上)|
|*|カーソルがある位置の文字を検索(下)|
|#|カーソルがある位置の文字を検索(上)|
|:s/置換前/置換後|行を対象に一致した最初のものを置換|
|:s/置換前/置換後/g|行を対象に一致した全てを置換|
|:%s/置換前/置換後/g|ファイルを対象に一致した全てを置換|
|:%s/置換前/置換後/gc|ファイルを対象に一致した全てを置換(置換前に1つ1つ確認する)|
|%s/置換前/^M(Crtl + v → Enter)/g|ファイルを対象に置換前文字列を改行に置換|

### 差分比較
|コマンド|説明|
|:--|:--|
|:diffsplit 差分を取りたいファイル(ファイルパス含む)|ウィンドウを上下に分割して差分を表示|
|:vertical diffsplit 差分を取りたいファイル(ファイルパス含む)|ウィンドウを左右に分割して差分を表示|

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
|gt|右のタブへ移動する|
|gT|左のタブへ移動する|
|[数字]gt|左から[数字]番目のタブへ移動する|
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
|:terminal|MacVim上でterminalを表示する|
|exit → Cmd + w|MacVim上で表示したterminalを消す|
|:set wrap|自動折り返しon|
|:set nowrap|自動折り返しoff|

### MacVimショートカット
|コマンド|説明|
|:--|:--|
|cmd + shft + -|文字を大きくする|
|cmd + -|文字を小さくする|



