# cssアニメーションの演習です
## 目的
* cssアニメーションを使うことで、簡単にサイトに動きが付けられることを理解する
* transformとtransitionの使い方を理解する

## 覚えて欲しいこと
### transition
要素の2つの状態の変化に動きをつけることができる
https://developer.mozilla.org/ja/docs/Web/CSS/transition
#### 構文
```
/** プロパティ名に指定したプロパティの変化を指定した時間かけて変化させる **/
transition: {プロパティ名} {時間};

/** 上記に加えて、遅延時間経過後にアニメーションを開始する **/
transition: {プロパティ名} {時間} {遅延};

/** 時間関数を指定することで動きに変化をつけることができる **/
transition: {プロパティ名} {時間} {時間関数};

transition: {プロパティ名} {時間} {時間関数} {遅延} {時間関数}

/** 
プロパティ名にはcssのプロパティのほか、allとすることで全てのプロパティに対して変化に動きをつけることができる
**/
```

### transform
要素の拡大縮小、回転、斜めにする、移動させることができるプロパティ
https://developer.mozilla.org/ja/docs/Web/CSS/transform
#### 構文
よく使うもののみ取り上げる
```
/** 回転 **/
transform: rotate(90deg); /** 90度回転させる **/
/** 拡大縮小 **/
transform: scale(.5) /** 半分の大きさにする **/
/** 移動 **/
transform: translate({x座標} {y座標})
```

## transformを使わないアニメーション
キーフレームアニメーションという手法で動きをつけることもできる。
こちらの方が細かく動きを指定できるので、細かい動きや、複雑な動きのときはこちらを使用する
https://developer.mozilla.org/ja/docs/Web/CSS/@keyframes