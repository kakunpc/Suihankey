# はじめに

このたびは、「すいはんきー」をお買い上げいただきまして誠にありがとうございます。  
この製品はPC向けオンラインゲームでの使用を想定して作られましたゲーム向けキーボードです。  
リバーシブル基板を採用しており、2つセットと追加パーツをお買い上げ頂いた方は、36キーの小さめな左右分割式キーボードとしてもご利用いただけます。

ファームウェアについては [QMK Firmware](https://github.com/qmk/qmk_firmware) を採用しており、ご購入者自身で各キー割り当てを変更することが出来ます。

本製品は組み立てが必要なキットとなります。
組み立てにはネジ締めやハンダ付けが必要となりますので、予め工具を揃えておいてください。
また、本製品には含まれていないもので必要なものがございます、必要なパーツを確認の上ご自身でお好みのものを別途揃えてください。

# 目次

- 必要な工具
- 本製品に含まれるパーツ一覧
- 本製品に含まれていない必要なパーツ一覧と主な購入先
- 本体の組み立て
- 基本ファームウェアの書き込み
- QMK Configuratorでファームウェアを作る
- 36キーキーボードとして使うときの注意事項

# 必要な工具
- ハンダゴテ https://www.amazon.co.jp/dp/B006MQD7M4
- コテ台 https://www.amazon.co.jp/dp/B000TGNWCS
- ハンダ https://www.amazon.co.jp/dp/B0029LGAJI
- ピンセット https://www.amazon.co.jp/dp/B002A5VG2E
- ニッパー https://www.amazon.co.jp/dp/B001D7TE2E
- 精密ドライバー https://www.amazon.co.jp/dp/B000CED236
- ワイヤーストリッパー https://www.amazon.co.jp/dp/B004OR7BQ6

## あると便利なもの
- テスター https://www.amazon.co.jp/dp/B06XPFRCGQ
- ヘッドルーペ https://www.amazon.co.jp/dp/B002T8EXVS
- ハンダ吸い取り線 https://www.amazon.co.jp/dp/B001PR1KPQ

# 本製品に含まれるパーツ一覧

|名前|個数| |
|:-----:|:----:|:----:|
|PCB|3枚||
|ダイオード|18個||
|M2 3mm貫通スペーサー|8個||
|M2 8mmネジ|8本||
|M2 3mmネジ|10本||
|M2 5mmネジ|2本||
|M2 5mmスペーサー|10個||
|M2 8mmスペーサー|2個||
|ゴム足|4つ||
|リセットスイッチ|1個||
|アクリル|1枚||

# 本製品に含まれていない必要なパーツ一覧と主な購入先

|名前|個数|入手先| |
|:-----:|:----:|:----:|:----:|
|ProMicro+コンスルー|1セット|遊舎工房( https://yushakobo.jp/shop/promicro-spring-pinheader/ )| |
|SSD1306|1個|遊舎工房( https://yushakobo.jp/shop/oled/ )| |
|MXキーソケット|18個|遊舎工房( https://yushakobo.jp/shop/a01ps/ )| |
|（任意）SK6812MINI|18個|遊舎工房( https://yushakobo.jp/shop/sk6812mini-35/ )| |
|（任意）ワイヤー5cmぐらい|3本|秋月電子通商( http://akizukidenshi.com/catalog/g/gP-06756/ )| |

# 本体の組み立て
TDB

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

