# はじめに

このたびは、「すいはんきー」をお買い上げいただきまして誠にありがとうございます。  
この製品はPC向けオンラインゲームでの使用を想定して作られましたゲーム向けキーボードです。    
リバーシブル基板を採用しており、2つセットと追加パーツをお買い上げ頂いた方は、36キーの小さめな左右分割式キーボードとしてもご利用いただけます。

ファームウェアについては [QMK Firmware](https://github.com/qmk/qmk_firmware) を採用しており、ご購入者自身で各キー割り当てを変更することが出来ます。

本製品は組み立てが必要なキットです。  
組立工程の中には、ハンダ付けや細いねじを締める工程があります。  
あらかじめ必要な工具（後述）を用意した上で、組立を始めてください。

また、本製品には含まれていないもので必要なものがございます、必要なパーツを確認の上ご自身でお好みのものを別途揃えてください。

# 目次

- [必要な工具](https://github.com/kakunpc/Suihankey#%E5%BF%85%E8%A6%81%E3%81%AA%E5%B7%A5%E5%85%B7)
- [本製品に含まれるパーツ一覧](https://github.com/kakunpc/Suihankey#%E6%9C%AC%E8%A3%BD%E5%93%81%E3%81%AB%E5%90%AB%E3%81%BE%E3%82%8C%E3%82%8B%E3%83%91%E3%83%BC%E3%83%84%E4%B8%80%E8%A6%A7)
- [本製品に含まれていない必要なパーツ一覧と主な購入先](https://github.com/kakunpc/Suihankey#%E6%9C%AC%E8%A3%BD%E5%93%81%E3%81%AB%E5%90%AB%E3%81%BE%E3%82%8C%E3%81%A6%E3%81%84%E3%81%AA%E3%81%84%E5%BF%85%E8%A6%81%E3%81%AA%E3%83%91%E3%83%BC%E3%83%84%E4%B8%80%E8%A6%A7%E3%81%A8%E4%B8%BB%E3%81%AA%E8%B3%BC%E5%85%A5%E5%85%88)
- [本体の組み立て](https://github.com/kakunpc/Suihankey#%E6%9C%AC%E4%BD%93%E3%81%AE%E7%B5%84%E3%81%BF%E7%AB%8B%E3%81%A6)
- [基本ファームウェアの書き込み](https://github.com/kakunpc/Suihankey#%E5%9F%BA%E6%9C%AC%E3%83%95%E3%82%A1%E3%83%BC%E3%83%A0%E3%82%A6%E3%82%A7%E3%82%A2%E3%81%AE%E6%9B%B8%E3%81%8D%E8%BE%BC%E3%81%BF)
- [QMK Configuratorでファームウェアを作る](https://github.com/kakunpc/Suihankey#qmk-configurator%E3%81%A7%E3%83%95%E3%82%A1%E3%83%BC%E3%83%A0%E3%82%A6%E3%82%A7%E3%82%A2%E3%82%92%E4%BD%9C%E3%82%8B)
- [36キーキーボードとして使うときの注意事項](https://github.com/kakunpc/Suihankey#36%E3%82%AD%E3%83%BC%E3%82%AD%E3%83%BC%E3%83%9C%E3%83%BC%E3%83%89%E3%81%A8%E3%81%97%E3%81%A6%E4%BD%BF%E3%81%86%E3%81%A8%E3%81%8D%E3%81%AE%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A0%85)

# 必要な工具
- ハンダゴテ https://www.amazon.co.jp/dp/B006MQD7M4
- コテ台 https://www.amazon.co.jp/dp/B000TGNWCS
- ハンダ https://www.amazon.co.jp/dp/B0029LGAJI
- ピンセット https://www.amazon.co.jp/dp/B002A5VG2E
- ニッパー https://www.amazon.co.jp/dp/B001D7TE2E
- 精密ドライバー https://www.amazon.co.jp/dp/B000CED236
- ワイヤーストリッパー https://www.amazon.co.jp/dp/B004OR7BQ6

## あると便利なもの
- テスタ https://www.amazon.co.jp/dp/B06XPFRCGQ
- ヘッドルーペ https://www.amazon.co.jp/dp/B002T8EXVS
- ハンダ吸い取り線 https://www.amazon.co.jp/dp/B001PR1KPQ

# 本製品に含まれるパーツ一覧

|名前|個数| |
|:-----:|:----:|:----:|
|PCB|1枚|![main](https://github.com/kakunpc/Suihankey/blob/master/images/main.jpg?raw=true)|
|トッププレート|1枚|![top](https://github.com/kakunpc/Suihankey/blob/master/images/top.jpg?raw=true)|
|ボトムプレート|1枚|![bottom](https://github.com/kakunpc/Suihankey/blob/master/images/bottom.jpg?raw=true)|
|ダイオード|18個|![diode](https://github.com/kakunpc/Suihankey/blob/master/images/diode.jpg?raw=true)|
|M2 3mm貫通スペーサー|8個|![m-3sp](https://github.com/kakunpc/Suihankey/blob/master/images/m-3sp.jpg?raw=true)|
|M2 8mmネジ|8本|![m2-8mm](https://github.com/kakunpc/Suihankey/blob/master/images/m2-8mm.jpg?raw=true)|
|M2 3mmネジ|10本|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-3mm.jpg?raw=true)|
|M2 5mmネジ|2本|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-5mm.jpg?raw=true)|
|M2 5mmスペーサー|10個|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-5sp.jpg?raw=true)|
|M2 8mmスペーサー|2個|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-8sp.jpg?raw=true)|
|ゴム足|4つ|![rubber](https://github.com/kakunpc/Suihankey/blob/master/images/rubber.jpg?raw=true)|
|リセットスイッチ|1個|![reset](https://github.com/kakunpc/Suihankey/blob/master/images/reset.jpg?raw=true)|
|アクリル|1枚|![plate](https://github.com/kakunpc/Suihankey/blob/master/images/plate.jpg?raw=true)|

# 本製品に含まれていない必要なパーツ一覧と主な購入先

|名前|個数|入手先| |
|:-----:|:----:|:----:|:----:|
|ProMicro+コンスルー|1セット|遊舎工房( https://yushakobo.jp/shop/promicro-spring-pinheader/ )|![pcb](https://github.com/kakunpc/Suihankey/blob/master/images/promico.jpg?raw=true)|
|SSD1306|1個|遊舎工房( https://yushakobo.jp/shop/oled/ )|![ssd1306](https://github.com/kakunpc/Suihankey/blob/master/images/ssd1306.jpg?raw=true)|
|MXキーソケット|18個|遊舎工房( https://yushakobo.jp/shop/a01ps/ )|![kailhchoc](https://github.com/kakunpc/Suihankey/blob/master/images/kailhchoc.jpg?raw=true)|
|（任意）SK6812MINI|18個|遊舎工房( https://yushakobo.jp/shop/sk6812mini-35/ )|![sk6812mini](https://github.com/kakunpc/Suihankey/blob/master/images/sk6812mini.jpg?raw=true)|
|（任意）ワイヤー5cmぐらい|3本|秋月電子通商( http://akizukidenshi.com/catalog/g/gP-11640/ )| |

# 本体の組み立て

## 0.PCBの見かた（表裏、上下左右）

## 1. ダイオードを取り付け

まず、ダイオードを取り付けていきます。

ダイオードとは、電気の流れの向きを一定にする仕組みのものです。  
水で表現すると水流の向きを制御し、逆向きに水が流れることを防ぎます。

この特徴からダイオードには表面に細い線の印刷がされています。  
肉眼では見辛いときはライトの向きを変えたり虫眼鏡で確認してください。

**逆向きに取り付けてしまうと、そのキーは反応しなくなってしまいます。**

ダイオードを取り付けるPCBの面は、裏側になります。

ダイオードの端に細い線が通っている方と、 
PCB側の `コ` の字型の線がある方を同じ向きに揃えてハンダ付けしていきます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/1.jpg?raw=true)

ダイオードを取り付けるところにあらかじめはんだを盛っておきます。これを予備はんだといいます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/2.jpg?raw=true)

その後、先程予備ハンダしたところを半田ゴテで温めながら、ピンセットを使ってダイオードの取り付けていきます。  
うまく位置を合わせながらピンセットで固定しながら半田ゴテを外し、ハンダが固まるまで約1秒ピンセットを固定し、ハンダが固まったらピンセットを離し片足の取り付けが完了です。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/3.jpg?raw=true)

その後、もう片方の足をはんだ付けします。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/4.jpg?raw=true)

これを18個分行っていきます。


すべてのダイオードをはんだ付けすると次の写真のようになります。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/5.jpg?raw=true)

ダイオードハンダ付けの参考動画です。  
https://twitter.com/Salicylic_acid3/status/1108798243142434816

## 2. リセットスイッチの取り付け
次に、リセットスイッチを取り付けます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/1.jpg?raw=true)

リセットスイッチも同じく先に片足だけ予備ハンダします。
その後、ピンセットを使いながらスイッチの片足をはんだ付けします。  
はんだ付けできたら、もう片足と横の方もしっかりはんだ付けしていきます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/2.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/3.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/4.jpg?raw=true)

## 3. キースイッチ用のソケットをはんだ付けする
KailhChocソケットをはんだ付けします。

穴が複数空いており複雑になっています。
向きを間違えないよう、PCBの枠線に合うように置いてはんだ付けしていきます。

***ソケットの向き、PCBの面を間違えてしまうとキースイッチがはまらなくなってしまいます。写真を見ながら慎重に作業してください。***

![image](https://github.com/kakunpc/Suihankey/blob/master/images/3/2.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/3/3.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/3/4.jpg?raw=true)
すべてのソケットをはんだ付けすると上の写真のようになります。


## 4. OLEDのジャンパする

ジャンパとは基板の一部をショートさせ電通させる事を言います。

PCBを表面にし、 `SDA,SCL,VCC,GND` のところをハンダでショートさせます。  
次の写真のまるで囲ってある部分のちょっと下に印字されています。

***裏面ではないです。間違えないようにしてください。***  
***また、両面ともショートさせないでください。***

![image](https://github.com/kakunpc/Suihankey/blob/master/images/4/1.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/4/2.jpg?raw=true)


## 5. OLEDソケットを付ける

先程ジャンパしたところの下の位置にOLEDソケットをつけてはんだ付けしていきます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/5/1.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/5/2.jpg?raw=true)

## 6. RGBLEDをつける（オプション）

この作業の必要のない方は [(8. ネジを付ける)](https://github.com/kakunpc/Suihankey#8-%E3%83%8D%E3%82%B8%E3%82%92%E4%BB%98%E3%81%91%E3%82%8B) までの作業を省略してください。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/6/1.jpg?raw=true)

作業を行う前に半田ゴテの温度を230度まで下げます。  
半田ゴテの温度が高い状態で作業するとLEDを熱で破壊してしまう場合があります。  
これを防ぐために、コテ先の温度を下げるのを忘れないように注意してください。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/6/2.jpg?raw=true)

RGBLEDの切込みと、PCBの枠で囲った位置が合うよう向きを合わせてはんだ付けしていきます。
このとき、ダイオードでやったのと同じで一箇所だけ予備ハンダし、ピンセットを使ってハンダ付けしてください。

***このとき、なるべく慌てず素早く作業しましょう。温度が低くても長時間温め続けてしまうとLEDを破損させる原因となります。***

![image](https://github.com/kakunpc/Suihankey/blob/master/images/6/3.jpg?raw=true)

## 7. ボトムプレートとPCBをワイヤーでつなぐ（オプション）

ワイヤーを5cm～7cmぐらいの長さに揃えて切り、両端から３ミリを目安にワイヤーストリッパーなどを使って被覆を剥ぎます。

その後、上から同じ位置に合うようにワイヤーを刺し、はんだ付けします。

□から `VCC,LED,GND` の順になっています。


![image](https://github.com/kakunpc/Suihankey/blob/master/images/7/1.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/7/2.jpg?raw=true)

## 8. ネジを付ける
ひっくり返す作業が必要となりますのでカッターマットなどを用意してください。
ない場合はテープなどで代用可能です。

トッププレートに `M2 8mmネジ` を8箇所全てのネジ穴に指します。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/1.jpg?raw=true)

その後カッターマットなどを利用してネジ穴から落ちないようひっくり返します。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/2.jpg?raw=true)

ひっくり返したら、 `M2 3mm 貫通スペーサー` を8箇所と通します。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/3.jpg?raw=true)

その後、PCBを付けて、 `M2 5mm スペーサー` で固定します。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/4.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/5.jpg?raw=true)

8箇所すべて固定しネジが落ちない状況になったら、再度ひっくり返し、PCBに `M2 8mmスペーサー` を通します。その後反対側を `M2 5mm スペーサー` で固定します。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/6.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/7.jpg?raw=true)

最後にボトムプレートをとりつけ `M2 3mm ネジ` で10箇所固定します。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/8.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/8/9.jpg?raw=true)

## 9. ProMicroにコンスルーをつける
ProMicroとコンスルーを準備します。
遊舎工房様で購入した場合は、ピンヘッダとコンスルーの両方がついてきます。
そのうち、写真の下側のほうがコンスルーでこちらの方を使っていきます。 (上の方は不要なので破棄するかよしなにしてください)

![image](https://user-images.githubusercontent.com/5952961/59026138-aec00a00-8890-11e9-8fba-5ff7336ee15c.jpg)

ProMicroの部品が実装されている面にコンスルーを差し込みます。
コンスルーの小さな小窓がProMicroに近い側であること、手前奥ともに小窓が見えていることを確認したらひっくり返します。

![image](https://user-images.githubusercontent.com/5952961/59015614-5b42c180-887a-11e9-92bd-fa32baa3fef1.JPG)
![image](https://user-images.githubusercontent.com/5952961/59015616-5da51b80-887a-11e9-8408-a7d9d0e1b51e.JPG)

## 10. PCBにProMicroを取り付ける

この状態でPCBにProMicroを取り付けます。  
12ピンのProMicroに対し13個穴が空いてますが、これはBLEMicroPro用に準備されています。

取り付けるときは白い枠線にピッタリ合うよう、下の線に合わせて取り付けます。

その後もう一度しっかり刺さってるか確認し、ProMicroをはんだ付けします。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/10/1.jpg?raw=true)

## 11. OLEDをつける
最後にOLEDをハンダ付けします。
ピンヘッダをソケットに差し込み、その上にOLEDを乗せ、そのままはんだ付けします。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/11/1.jpg?raw=true)

## 12. OLED保護アクリルを取り付ける
アクリルについている紙を剥がします。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/12/1.jpg?raw=true)

次にOLEDの保護シートを剥がし、 `M2 5mm ネジ` でアクリルを固定します。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/12/2.jpg?raw=true)

## 13. ゴム足をつける
キーボードと机を保護するためにゴム足を取り付けます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/13/1.jpg?raw=true)

## 14. キースイッチとキーキャップを指す

まずキースイッチを付けます。  
キースイッチには足が出ており、そちらをキーソケットに接続することで電通することが出来ます。
写真の赤丸で囲った部分が合うようにキースイッチをまっすぐ差し込みます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/14/1.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/14/2.jpg?raw=true)

すべてのキースイッチを差し込んだあと、キーキャップを付けていきます。  
つけるキースイッチの種類によって向きがありますので、確認しながら付けましょう。  
キーキャップには十字の切れ込み、キースイッチには十字の軸がついています。  
そちらの向きを確認しながらまっすぐ差し込んでいってください。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/14/3.jpg?raw=true)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/14/4.jpg?raw=true)

これで本体は完成です。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/14/5.jpg?raw=true)

# 基本ファームウェアの書き込み

まずは動作確認のため基本ファームウェアを書き込みます。

書き込みには [qmk_toolbox](https://qmk.fm/toolbox/) を使用します。
[こちら](https://github.com/qmk/qmk_toolbox/releases) から最新版をダウンロードし任意の場所に保存します。

次に、[こちら](https://github.com/kakunpc/Suihankey/releases/)からSuihankey用のファームウェアをダウンロードし任意の場所に保存します。 (suihankey_rev1_default.hex)

その後qmk_toolboxを起動します。

起動したら次のように設定します。

- `Local File` を先程保存したSuihankey用のファームウェアを指定します
- `Microcontroller` を `atmega42u4` を指定します。
- `Auto-Flash` にチェックを入れます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/qmk_toolbox/1.jpg?raw=true)

準備ができたら、USBでPCとSuihankeyを接続します。
その後、リセットスイッチを押してしばらくまちます。

`Thank you.` と画面に出たら完了です。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/qmk_toolbox/2.jpg?raw=true)

デフォルトファームウェアはこの様になっています。
実際にボタンをして正しく動作するか確認しましょう。

**FUNCTION・NUMBER・COMANDに関しては、OLEDディスプレイの文字が変化します。**

![image](https://github.com/kakunpc/Suihankey/blob/master/images/qmk_toolbox/3.jpg?raw=true)

# QMK Configuratorでファームウェアを作る
TDB

# 36キーキーボードとして使うときの注意事項
- 4.7kΩの抵抗が2つと、4ピンのジャックのハンダ付けが別途必要になります。  
- TRRSケーブルが必要です。
    - どれも遊舎工房とAitendoで購入可能です。
- 左右どちらにもOLEDを接続はできますが、アドレスが同じなため2つとも同じ表示となります。左右う別々の表示はできません。
- OLEDを利用する場合左右で別々のファームウェアを準備する必要があります。
    - マスタ側にOLEDをON、スレーブ側ではOLEDをOFFにするだけです。
