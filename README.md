# ロボホンのロブリックアプリで動かせるプログラム

## インストール方法

* [ZIPファイル](https://github.com/3110/robohon-robrick/archive/v0.0.1.zip)をダウンロードします。
* ダウンロードしたZIPファイルを適当なフォルダに展開します。
* ロボホンでロブリックアプリを起動します。  
  <a href="https://gyazo.com/4c6059c6ee7deace2185d194e2587e22"><img src="https://i.gyazo.com/4c6059c6ee7deace2185d194e2587e22.png" alt="ロブリックアプリアイコン" width="180"/></a>
* ロボホンの画面に表示されている文字列をWebブラウザのアドレスバーに入力してください（詳細は[利用マニュアル](https://robohon.com/apps/robrick/manual101.pdf)の10ページを参照）  
  <a href="https://gyazo.com/03ab2d8be37ce7ec4e92773205f10020"><img src="https://i.gyazo.com/03ab2d8be37ce7ec4e92773205f10020.png" alt="ロブリック起動画面" width="180"/></a>  
  <a href="https://gyazo.com/2c4fa167263e0cc0f90c2911ffe87f22"><img src="https://i.gyazo.com/2c4fa167263e0cc0f90c2911ffe87f22.png" alt="Google Chromeでの例" width="800"/></a>
* Webブラウザにロブリックの画面が表示されます。  
  <a href="https://gyazo.com/826959a2535c9b253b6dd647bc01217a"><img src="https://i.gyazo.com/826959a2535c9b253b6dd647bc01217a.png" alt="ロブリック画面" width="800"/></a>
* 画面左下にある「設定」ボタンを押し，「保存先」が「デバイス」になっていることを確認します。「保存先」はプログラムを読み込むときの読み込み先としても使われます。設定画面を閉じるときは右上の「×」を押します。    
  <a href="https://gyazo.com/0f9dbbe00a22f19ba0c1bcd32933efa0"><img src="https://i.gyazo.com/0f9dbbe00a22f19ba0c1bcd32933efa0.png" alt="設定画面" width="800"/></a>
* 画面下にある「読み込み」ボタンを押して，ZIPファイルを展開したフォルダにあるXML（例えばクイズアプリなら`quiz-app.xml`）を選択し，「開く」ボタンを押します。  
  <a href="https://gyazo.com/d3c96694a53cbd7332463c5134e491a2"><img src="https://i.gyazo.com/d3c96694a53cbd7332463c5134e491a2.png" alt="ファイルの選択" width="800"/></a>
* アプリが読み込まれます。  
  <a href="https://gyazo.com/d02c36f6947f9f1edadbaf680394481f"><img src="https://i.gyazo.com/d02c36f6947f9f1edadbaf680394481f.png" alt="アプリ読み込み完了" width="800"/></a>
* 「スタート」ボタンを押すと実行されます。アプリを変更したりしていろいろ試してみましょう。
    * この場合，ブラウザへ情報を送りながら実行するため，実行中に遅延が生じることがあります。
* カスタマイズが完了したら，「ロボホンに送信」ボタンを押してロボホンに送信します。わかりやすい名前（例えば「クイズアプリ」）に変更しましょう。  
  <a href="https://gyazo.com/c9a890b15673b7ef113c425c25db623b"><img src="https://i.gyazo.com/c9a890b15673b7ef113c425c25db623b.png" alt="ロボホンに送信" width="800"/></a>
* 「保存しました」と表示されたら「OK」ボタンを押します。  
  <a href="https://gyazo.com/03ee151ce2e646ee79d52c9491301bd2"><img src="https://i.gyazo.com/03ee151ce2e646ee79d52c9491301bd2.png" alt="保存完了" width="800"/></a>
* ロボホンの画面で「ロブリック実行」アプリを起動します。  
  <a href="https://gyazo.com/4c6059c6ee7deace2185d194e2587e22"><img src="https://i.gyazo.com/4c6059c6ee7deace2185d194e2587e22.png" alt="ロブリックアプリアイコン" width="180"/></a>
* 「保存したときに付けた名前.js」が表示されていることを確認し，再生ボタンを押すとアプリが実行されます。  
  <a href="https://gyazo.com/7caf6342aef96d50caaf5d9db09ca48f"><img src="https://i.gyazo.com/7caf6342aef96d50caaf5d9db09ca48f.png" alt="Image from Gyazo" width="180"/></a>

## クイズアプリ（`quiz-app.xml`）

### 特徴

* クイズの作成は「質問」「選択肢の一覧（最初が正解）」を追加するだけでできます。
* クイズ名を指定できます。
* 出題数を変えられます。
* 出題はランダム・順番通りが選べます。
* 選択肢の数は問題ごとに変えられます。
* 選択肢の提示はランダム（出題ごとに順番が変わる）です。
* 聞きとれないときの聞き返し回数を設定できます。

### カスタマイズ

<a href="https://gyazo.com/bd1d86d315a24198a62ecedca2e294a5"><img src="https://i.gyazo.com/bd1d86d315a24198a62ecedca2e294a5.png" alt="カスタマイズ" width="360"/></a>

### クイズ作成

* 「クイズ一覧取得」関数にあるリストを編集します。  
  <a href="https://gyazo.com/5e53e42df63c0f7d60fbbc6229a607f5"><img src="https://i.gyazo.com/5e53e42df63c0f7d60fbbc6229a607f5.png" alt="クイズ一覧" width="800"/></a>
* 右側がギザギザになっているブロックには，いくつかのブロックがまとめられています。そのブロックを右クリックし，メニューの「ブロックを展開する」を選択すると表示されます。  
  <a href="https://gyazo.com/8ccafbecb34bbb4dc66ec2ba31fd1b54"><img src="https://i.gyazo.com/8ccafbecb34bbb4dc66ec2ba31fd1b54.gif" alt="Image from Gyazo" width="800"/></a>
* クイズ1問分のデータは以下のようになっています。  
  <a href="https://gyazo.com/c71fc488cf05ed08c549d6d230aae470"><img src="https://i.gyazo.com/c71fc488cf05ed08c549d6d230aae470.png" alt="Image from Gyazo" width="800"/></a>
