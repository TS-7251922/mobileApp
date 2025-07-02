# モバイルアプリ開発　まとめ  
末尾に半角スペースで改行  
## widgetについて
▶︎StatelessWidget(ステイトレス)について  
 　一度構築すると変化しない。  
 　外から渡されたデータだけで表示される。  
 　状態管理の必要がない場合に使用。
   
▶︎StatefulWidget(ステイトフル)について   
 　内部に状態（State）を持ち、変化させることができる。  
 　setState() を使うと build() が再実行され、UIが更新される。  
 
・レイアウト  
▶︎Column と Row  
 　縦方向／横方向に子ウィジェットを並べる。  
▶︎MainAxisAlignment と CrossAxisAlignment  
 　主軸（Column：縦、Row：横）と交差軸方向の揃え位置を制御  
▶︎Container  
 　padding・margin・背景色・境界線・幅・高さなどのプロパティを指定可能  
▶︎Expanded ウィジェット  
 　親の空きスペースを占有する。Flexibleとの違いも説明  

・画像  
 ▶︎AssetImage, NetworkImage, Image.asset, Image.network  
 　アセットの配置場所やネットワーク画像の読み込み  

・ボタンと処理  
▶︎ElevatedButton, TextButton, IconButton   
　onPressed や onTap でユーザーの操作を受け取り、画面制御や状態更新を行う  

・State（状態管理）  
▶︎setState  
　状態を変更した後に setState() を呼ぶことで build() が再実行され、UIに反映される  

 ### 主なウィジェット
例）ウィジェット名　　概要	　　主な用途  
▶︎TextField　　テキスト入力欄　　名前やメッセージなどの文字入力  
▶︎Checkbox　　複数選択可能なチェックボックス　　同意確認・オプション選択など  
▶︎Switch　　ON/OFF を切り替えるスイッチ　　設定の有効・無効など  
▶︎Radio　　単一選択のラジオボタン　　性別選択など、一つだけ選ばせたいとき  
▶︎Slider　　数値をスライドバーで調整　　音量、明るさ、数値設定  
▶︎RangeSlider　　数値の範囲をスライドで選択　　最小値～最大値の範囲指定  
▶︎DropdownButton　　プルダウン選択　　カテゴリ選択、都道府県など  
▶︎DatePicker　　カレンダー形式で日付選択　　誕生日、スケジュール入力など  
▶︎TimePicker　　時計形式で時刻選択　　アラーム、予定時間など  

## データアクセスについて  
・ファイルアクセス  
　▶︎fileクラスを使い、端末内の読み書きを行う 
 　- path_provider パッケージで、アプリのドキュメントディレクトリなどへのアクセスパスを取得  
 　- テキストファイルの読み込み・保存の基本フローと例示コードを掲載
 　- リソースフォルダ内のファイルの読み込み  
・設定情報  
　▶︎ shared_preferences パッケージを追加・導入  
 　　- キーと値で構成されたプリミティブ型の永続設定保存  
 　　- getString, setBool, removeの読み書き操作  
 　　- アプリの設定保存  
・ネットワークアクセス  
　▶︎ HttpClient クラスを使い、HTTP通信を行う  
　　‑ GETリクエストでWebサイトからデータ取得、POSTリクエストでデータ送信  
　　‑ 通信結果を受け取ってUIに反映する流れと基本コードを掲載  
　　‑ 応答の処理・エラーハンドリング・ステータスチェックのポイントも説明  
・


 
 
