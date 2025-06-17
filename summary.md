# モバイルアプリ開発　まとめ  
末尾に半角スペースで改行  
## 一章 〜widget〜
▶︎StatelessWidget(ステイトレス)について  
 →一度構築すると変化しない。  
 →外から渡されたデータだけで表示される。  
 →状態管理の必要がない場合に使用。
   
▶︎StatefulWidget(ステイトフル)について   
 →内部に状態（State）を持ち、変化させることができる。  
 →setState() を使うと build() が再実行され、UIが更新される。  
 
＞レイアウト  
▶︎Column と Row  
  →縦方向／横方向に子ウィジェットを並べる。  
▶︎MainAxisAlignment と CrossAxisAlignment  
  →主軸（Column：縦、Row：横）と交差軸方向の揃え位置を制御  
▶︎Container  
  →padding・margin・背景色・境界線・幅・高さなどのプロパティを指定可能  
▶︎Expanded ウィジェット  
  →親の空きスペースを占有する。Flexibleとの違いも説明  


 
