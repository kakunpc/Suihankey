# はじめに

このたびは、「すいはんきー」をお買い上げいただきまして誠にありがとうございます。  
この製品はPC向けオンラインゲームでの使用を想定して作られましたゲーム向けキーボードです。  
リバーシブル基板を採用しており、2つセットと追加パーツをお買い上げ頂いた方は、36キーの小さめな左右分割式キーボードとしてもご利用いただけます。

ファームウェアについては [QMK Firmware](https://github.com/qmk/qmk_firmware) を採用しており、ご購入者自身で各キー割り当てを変更することが出来ます。

本製品は組み立てが必要なキットとなります。
組み立てにはネジ締めやハンダ付けが必要となりますので、予め工具を揃えておいてください。
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
|PCB|1枚|![pcb](https://github.com/kakunpc/Suihankey/blob/master/images/pcb.jpg)|
|トッププレート|1枚||
|ボトムプレート|1枚||
|ダイオード|18個|![diode](https://github.com/kakunpc/Suihankey/blob/master/images/diode.jpg)|
|M2 3mm貫通スペーサー|8個|![m-3sp](https://github.com/kakunpc/Suihankey/blob/master/images/m-3sp.jpg)|
|M2 8mmネジ|8本|![m2-8mm](https://github.com/kakunpc/Suihankey/blob/master/images/m2-8mm.jpg)|
|M2 3mmネジ|10本|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-3mm.jpg)|
|M2 5mmネジ|2本|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-5mm.jpg)|
|M2 5mmスペーサー|10個|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-5sp.jpg)|
|M2 8mmスペーサー|2個|![image](https://github.com/kakunpc/Suihankey/blob/master/images/m2-8sp.jpg)|
|ゴム足|4つ|![rubber](https://github.com/kakunpc/Suihankey/blob/master/images/rubber.jpg)|
|リセットスイッチ|1個|![reset](https://github.com/kakunpc/Suihankey/blob/master/images/reset.jpg)|
|アクリル|1枚|![plate](https://github.com/kakunpc/Suihankey/blob/master/images/plate.jpg)|

# 本製品に含まれていない必要なパーツ一覧と主な購入先

|名前|個数|入手先| |
|:-----:|:----:|:----:|:----:|
|ProMicro+コンスルー|1セット|遊舎工房( https://yushakobo.jp/shop/promicro-spring-pinheader/ )|![pcb](https://github.com/kakunpc/Suihankey/blob/master/images/promico.jpg)|
|SSD1306|1個|遊舎工房( https://yushakobo.jp/shop/oled/ )|![ssd1306](https://github.com/kakunpc/Suihankey/blob/master/images/ssd1306.jpg)|
|MXキーソケット|18個|遊舎工房( https://yushakobo.jp/shop/a01ps/ )|![kailhchoc](https://github.com/kakunpc/Suihankey/blob/master/images/kailhchoc.jpg)|
|（任意）SK6812MINI|18個|遊舎工房( https://yushakobo.jp/shop/sk6812mini-35/ )|![sk6812mini](https://github.com/kakunpc/Suihankey/blob/master/images/sk6812mini.jpg)|
|（任意）ワイヤー5cmぐらい|3本|秋月電子通商( http://akizukidenshi.com/catalog/g/gP-11640/ )| |

# 本体の組み立て

## 1. ダイオードを取り付け

まず、ダイオードを取り付けていきます。  
ダイオードを取り付けるPCBの面は、裏側になります。
ダイオードには向きがありますので注意して取り付けてください。

ダイオードの端に細い線が通っている方と、 
PCB側の `コ` の字型の線がある方を同じ向きに揃えてハンダ付けしていきます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/1.jpg)

取り付けるときは、まず片側に予備ハンダをします。  
その後、先程予備ハンダしたところを半田ゴテで温めながら、ピンセットを使ってダイオードの取り付けていきます。  
うまく位置を合わせながらピンセットで固定しながら半田ゴテを外し、ハンダが固まるまでピンセットを固定し、ハンダが固まったら片足の取り付けが完了です。
これを18個分行っていきます。

その後、もう片方の足をはんだ付けします。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/2.jpg)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/3.jpg)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/4.jpg)

すべてはんだ付けするとこのようになります。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/1/5.jpg)

## 2. リセットスイッチの取り付け
次に、リセットスイッチを取り付けていきます。  
ダイオードと同じく裏側にはんだ付けしていきます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/1.jpg)

スイッチも同じく先に片足だけ予備ハンダします。
その後、ピンセットを使いながらスイッチの片足をはんだ付けします。  
上手くはんだ付けできたら、もう片足と横の方もしっかりはんだ付けしていきます。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/2.jpg)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/3.jpg)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/2/4.jpg)

## 3. ソケットを付ける
KailhChocソケットをつけていきます。
こちらも、裏面にはんだ付けします。

![image](https://github.com/kakunpc/Suihankey/blob/master/images/3/1.jpg)

穴が複数空いており複雑になっています。
向きを間違えないよう、PCBの枠線に合うように置いてはんだ付けしていきます。

***ソケットの向き、PCBの面を間違えてしまうとスイッチがはまらなくなってしまいます。写真を見ながら慎重に作業してください。***

![image](https://github.com/kakunpc/Suihankey/blob/master/images/3/2.jpg)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/3/3.jpg)
![image](https://github.com/kakunpc/Suihankey/blob/master/images/3/4.jpg)

## 4. OLEDのジャンパする
PCBを表面にし、 `SDA,SCL,VCC,GND` のところをハンダでジャンパしていきます。

***ここのジャンパは裏面ではないです。間違えないようにしてください。***

## 5. OLEDソケットを付ける

先程ジャンパしたところの下の位置にソケットをつけてはんだ付けしていきます。

## 6. RGBLEDをつける（オプション）
この作業の必要のない方は [(8. ネジを付ける)](https://github.com/kakunpc/Suihankey#8-%E3%83%8D%E3%82%B8%E3%82%92%E4%BB%98%E3%81%91%E3%82%8B) まで飛ばしてください。

まず半田ゴテの温度を下げます（230度ぐらいに）
半田ゴテの温度が高い状態で作業するとLEDを熱で壊してしまいますので、必ず下げてください。

LEDの切込みと、PCBの枠で囲った位置が合うよう向きを合わせてはんだ付けしていきます。
このとき、ダイオードでやったのと同じで一箇所だけ予備ハンダし、ピンセットを使ってハンダ付けしてください。

***このとき、なるべく慌てず素早く作業しましょう。温度が低くても長時間温め続けてしまうとLEDの故障の原因となります。***

## 7. ボトムプレートとPCBをワイヤーでつなぐ（オプション）

ワイヤーを5cm～7cmぐらいの長さに揃えて切り、端から数ミリワイヤーストリッパーなどを使って剥ぎます。

その後、上から同じ位置に合うようにワイヤーを刺し、はんだ付けします。

□から `VCC,LED,GND` の順になっています。

## 8. ネジを付ける
ひっくり返す作業が必要となりますのでカッターマットなどを用意してください。
ない場合はテープなどで代用可能です。

トッププレートに `M2 8mmネジ` を8箇所全てのネジ穴に指します。
その後カッターマットなどを利用してネジ穴から落ちないようひっくり返します。

ひっくり返したら、 `M2 3mm 貫通スペーサー` を8箇所と通します。

その後、PCBを付けて、 `M2 5mm スペーサー` で固定します。

8箇所すべて固定しネジが落ちない状況になったら、再度ひっくり返し、PCBに `M2 8mmスペーサー` を通します。その後反対側を `M2 5mm スペーサー` で固定します。

最後にボトムプレートをとりつけ `M2 3mm ネジ` で10箇所固定します。

## 9. ProMicroにコンスルーをつける
ProMicroとコンスルーを準備します。
遊舎工房様で購入した場合は、ピンヘッダとコンスルーの両方がついてきます。
そのうち、写真の下側のほうがコンスルーでこちらの方を使っていきます。 (上の方は不要なので破棄するかよしなにしてください)

コンスルーには向きがあり、小さな点がProMicro側に来るようにとりつけます。  
また、USBの受け口が内側になるようコンスルーをはんだ付けします。

## 10. PCBにProMicroを取り付ける
先程はんだ付けしたProMicroをPCBに取り付けていきます。
12ピンのProMicroに対し13個穴が空いてますが、これはBLEMicroPro用に準備されているものです。

取り付けるときは白い枠線にピッタリ合うよう、下の線に合わせて取り付けていきます。

## 11. OLEDをつける
最後にOLEDをハンダ付けします。
ピンヘッダをソケットに差し込み、その上にOLEDを乗せ、そのままはんだ付けします。

## 12. OLED保護アクリルを取り付ける
アクリルを上から剥がします。

次にOLEDの保護シートを剥がし、 `M2 5mm ネジ` でアクリルを固定します。

## 13. ゴム足をつける
ネジが傷をつけないように、ゴム足を取り付けます。

## 14. キースイッチとキーキャップを指す

向きに注意してキースイッチを指したあとキーキャップ付けていきます。
つけることが出来たらこれで本体は完成です。

# 基本ファームウェアの書き込み
TDB

# QMK Configuratorでファームウェアを作る
TDB

# 36キーキーボードとして使うときの注意事項
- 4.7kΩの抵抗が2つと、4ピンのジャックのハンダ付けが別途必要になります。  
- TRRSケーブルが必要です。
    - どれも遊舎工房とAitendoで購入可能です。
- 左右どちらにもOLEDを接続はできますが、アドレスが同じなため2つとも同じ表示となります。左右う別々の表示はできません。
- OLEDを利用する場合左右で別々のファームウェアを準備する必要があります。
    - マスタ側にOLEDをON、スレーブ側ではOLEDをOFFにするだけです。

