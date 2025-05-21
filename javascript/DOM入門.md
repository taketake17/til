
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

