
- querySelector <br>
  ボタンなどの要素を取得するための命令。指定したCSSセレクターに一致する最初の要素（Elementオブジェクト）を返します。

- addEventListener <br>
 JavaScriptでHTML要素に「イベントが発生したときに実行する処理（関数）」を登録するためのメソッドです。
たとえば「ボタンがクリックされたら処理を実行したい」「マウスを重ねたら動きをつけたい」といった場合に使います

```
{
    document.querySelector('button').addEventListener('mouseover',()=>{
        console.log('Clicked');
    });
}
```
これだと、マウスを重ねたときにコンソールログでClickedを表示させることができる。

基本構文
```
element.addEventListener(イベントの種類, 関数, オプション);
```

代表的なイベント構文
```
代表的なイベントの種類
イベント名	説明
click	クリックされたとき
mouseover	マウスが乗ったとき
keydown	キーボードのキーが押されたとき
submit	フォームが送信されたとき
change	入力欄の内容が変わったとき
load	ページや画像などの読み込みが完了したとき
```

- textContent <br>
テキスト内容」を取得・設定するためのプロパティです。

- toggle
  ```
  document.querySelector('p').classList.toggle('pink-bg');
  ```
  toggleでクラスがあるかないか切り替えられる

- 要素の取得
```
querySelector()
querySelectorAll()

getElementById()
getElementsByTagName()
getElemetsByClassName()
```

- createElement <br>
  JavaScriptで新しいHTML要素（タグ）を動的に作成するメソッドです。
主にdocument.createElement(タグ名)の形で使い、指定したタグ名の空の要素ノードを生成します

- appendChild insertBefore <br>
appendChildの使い方
appendChildは、親要素の「子要素リストの末尾」に新しい要素やノードを追加するメソッドです。
```
親要素.appendChild(追加したい要素);
```
insertBeforeの使い方
insertBeforeは、親要素の「指定した子要素（参照ノード）の直前」に新しい要素やノードを追加するメソッドです。
```
親要素.insertBefore(追加したい要素, 参照ノード);
```

- ラジオボタン

  html
  ```
  <input type="radio" name="color" value="red">Red 
    <input type="radio" name="color" value="blue">Blue 
    <input type="radio" name="color" value="green">Green
  ```
  main.js
  ```
  {
    document.querySelector('button').addEventListener('click',()=>{
        document.querySelectorAll('input').forEach((radio) =>{
                if(radio.checked === true){
                    alert(radio.value);
                }
            }
        )
    });
  }
  ```
  checkedがラジオボタンが選択されているかどうかを判定する。
  ラジオボタンの場合はforEachで取ってくる


  


