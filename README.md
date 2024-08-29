# trackmacro

![](./assets/pic1.JPEG)


* [monkeypad/pmw3360-breakout](https://github.com/monkeypad/pmw3360-breakout) を使用したトラックボール付きのマクロパッド
* キーボードに載せるお試しで作ったもので、以下の要件を満たすものを作った
    * monkeypad/pmw3360-breakout を使う
        * ピンソケットを使用して、ブレークアウトボードは使い回せるようにする
    * RP2040-Zero を使う
        * PCBの裏にはんだ付けする
            * pmw3360-breakout のセンサの高さが一番高くなるため、裏に配置できた
    * 分割キーボードとして機能させる
    * Chocソケットを使う
        * そのためにトッププレートとボトムプレートをスペーサーとねじで止める構造にする
    * ボールケース
        * 使い回せるような形状にする
        * ベアリングを使う

## 使用している部品

|部品|リンク|備考|
|---|---|---|
|PMW3360ブレークアウトボード|[monkeypad/pmw3360-breakout](https://github.com/monkeypad/pmw3360-breakout)|Booth で購入したら、ピンヘッダーもついていたけど、おそらく[これ](https://www.hirosugi-net.co.jp/shop/c/c12103211/)|
|ピンソケット 8ピン|https://www.hirosugi-net.co.jp/shop/c/c12111211/|FSR-41085-08 / 8.5mmのものを使用する|
|スペーサー M2 5mm|https://www.hirosugi-net.co.jp/shop/c/c10141012/|トッププレートとボトムプレートを止めるために使用する|
|ねじ M2 3mm|https://wilco.jp/products/F/FX-EB.html#page3|トッププレートとボトムプレートを止めるために使用する|
|タッピングネジ M2 8mm|https://wilco.jp/products/F/FPP-N.html|FPP-0000N / ボトムプレートとボールケースを止めるために使用する。JLCPCBのレジンに使えるタッピングネジ|
|RP2040-Zero|||
|ダイオード|||
|chocソケット|||
|TRRSソケット|||


### ボールケース関連

|部品|リンク|備考|
|---|---|---|
|ベアリング|https://amzn.asia/d/8OED4Yl|DDL-520ZZW52 / 内径2mm、外形5mm、幅2.5mm|
|ねじ M2 8mm||なべ小ねじならなんでもOK (頭径3.5mm、高さ1.3)|
|ナット M2||1種のナットを使っている|
|磁石 3x2mm|https://amzn.asia/d/gBrgy0N|ボールケースの上下に瞬間接着剤 (アロンアルフア EXTRA 速効多用途) でつけている|


## 3Dプリント

* JLCPCB の3Dプリントを使う想定
* stl 内の stl ファイルを SLA(Resin) で発注する


## LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。

> 表示 — あなたは 適切なクレジットを表示し、ライセンスへのリンクを提供し、変更があったらその旨を示さなければなりません。これらは合理的であればどのような方法で行っても構いませんが、許諾者があなたやあなたの利用行為を支持していると示唆するような方法は除きます。
>
> 非営利 — あなたは営利目的でこの資料を利用してはなりません。