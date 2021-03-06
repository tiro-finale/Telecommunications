<!--ts-->
   * [インターネットの特徴](#インターネットの特徴)
   * [パケット通信方式](#パケット通信方式)
   * [ネットワークシステムの階層化](#ネットワークシステムの階層化)
   * [プロトコルとインターフェイス](#プロトコルとインターフェイス)
   * [通信の分類(コネクションの型)](#通信の分類コネクションの型)
   * [応用層(Application Layer)](#応用層application-layer)
   * [トランスポート層(Transport Layer)](#トランスポート層transport-layer)
   * [ネットワーク層(Network Layer)](#ネットワーク層network-layer)
   * [データリンク層(Datalink Layer)](#データリンク層datalink-layer)
   * [物理層(Physical Layer)](#物理層physical-layer)
   * [ネットワーク層 IPv4(Internet Protocol)](#ネットワーク層-ipv4internet-protocol)
   * [IPv4アドレス](#ipv4アドレス)
   * [IPv4アドレスのビット構成](#ipv4アドレスのビット構成)
   * [IPv4のクラスレス(Class Less)アドレス](#ipv4のクラスレスclass-lessアドレス)
   * [特別なIPv4アドレス](#特別なipv4アドレス)
   * [ネットワークのアドレス計算](#ネットワークのアドレス計算)
   * [ドメイン名(Domain Name)](#ドメイン名domain-name)
   * [ドメイン名の階層構造](#ドメイン名の階層構造)
   * [ドメイン，IPアドレスの変換](#ドメインipアドレスの変換)
   * [DNSサーバ](#dnsサーバ)
   * [名前の正引きと逆引き](#名前の正引きと逆引き)
   * [IPデータグラムの送信](#ipデータグラムの送信)
   * [直接配送の手順](#直接配送の手順)
   * [MAC(イーサネット，物理)アドレス](#macイーサネット物理アドレス)
   * [ARP(Address Resolution Protocol)](#arpaddress-resolution-protocol)
   * [ARPの手順](#arpの手順)
   * [経路選択表](#経路選択表)
   * [経路選択(ルーティング)アルゴリズム](#経路選択ルーティングアルゴリズム)
   * [ルータ(ゲートウェイ)](#ルータゲートウェイ)
   * [間接配送の手順](#間接配送の手順)
   * [IPv4ヘッダ(IPv4 Header)](#ipv4ヘッダipv4-header)
   * [ICMP(Internet Control Message Protocol)](#icmpinternet-control-message-protocol)
   * [pingコマンド](#pingコマンド)
   * [ICMPの機能(ICMPエコー)](#icmpの機能icmpエコー)
   * [ICMPの機能(配送エラーの通知)](#icmpの機能配送エラーの通知)
   * [ICMPの機能(配送エラーの通知)](#icmpの機能配送エラーの通知-1)
   * [DHCP(Dynamic Host Configuration Protocol)](#dhcpdynamic-host-configuration-protocol)
   * [IPv6実用化の歴史](#ipv6実用化の歴史)
   * [ネットワーク層 IPv6](#ネットワーク層-ipv6)
   * [IPv6ヘッダの特徴](#ipv6ヘッダの特徴)
   * [IPv6のアドレス表記方法](#ipv6のアドレス表記方法)
   * [リンクローカルアドレス(LLA)](#リンクローカルアドレスlla)
   * [IPv6LLAのアドレス表記方法](#ipv6llaのアドレス表記方法)
   * [ユニークローカルアドレス(ULA)](#ユニークローカルアドレスula)
   * [グローバルアドレス(GUA)](#グローバルアドレスgua)
   * [インターフェースID(IFID)の生成](#インターフェースidifidの生成)
   * [EUI-64(Extended Unique ID 64 Bit)方式](#eui-64extended-unique-id-64-bit方式)
   * [IPv6アドレス(通信形態による分類)](#ipv6アドレス通信形態による分類)
   * [マルチキャストアドレス](#マルチキャストアドレス)
   * [特殊なIPv6アドレス](#特殊なipv6アドレス)
   * [ネットワークのアドレス](#ネットワークのアドレス)
   * [経路選択(Routing)](#経路選択routing)
   * [経路選択(ルーティング)アルゴリズム](#経路選択ルーティングアルゴリズム-1)
   * [データリンク層のアドレスの解決](#データリンク層のアドレスの解決)
   * [NDP(Neighbor Discovery Protocol)](#ndpneighbor-discovery-protocol)
   * [RS(Router Solicitation)メッセージ](#rsrouter-solicitationメッセージ)
   * [RA(Router Advertisement)メッセージ](#rarouter-advertisementメッセージ)
   * [ステートレスアドレス自動設定](#ステートレスアドレス自動設定)
   * [LLAの自動設定](#llaの自動設定)
   * [ULA，GUAの自動設定](#ulaguaの自動設定)
   * [応用層プログラムの識別: ポート番号](#応用層プログラムの識別-ポート番号)
   * [Well-Known Port](#well-known-port)
   * [トランスポート層 TCP](#トランスポート層-tcp)
   * [トランスポート層 UDP](#トランスポート層-udp)
   * [イーサネット](#イーサネット)
   * [100Base-TX](#100base-tx)
   * [1000Base-T](#1000base-t)
   * [UTP系イーサネットの分類](#utp系イーサネットの分類)
   * [イーサネットの通信形態](#イーサネットの通信形態)
   * [SW Hub](#sw-hub)
   * [Wi-Fi(無線LAN)](#wi-fi無線lan)
   * [周波数帯域(2.4GHz帯)](#周波数帯域24ghz帯)
   * [周波数帯域(5GHz帯)](#周波数帯域5ghz帯)
   * [Wi-Fi(無線LAN)の方式](#wi-fi無線lanの方式)
   * [IPv6のまとめ](#ipv6のまとめ)
      * [IPv6のフィールド分割によるアドレス構造](#ipv6のフィールド分割によるアドレス構造)
      * [ユニキャストのフィールド](#ユニキャストのフィールド)
         * [ユニークローカル・ユニキャストアドレス](#ユニークローカルユニキャストアドレス)
         * [リンクローカル・ユニキャストアドレス](#リンクローカルユニキャストアドレス)
         * [グローバル・ユニキャストアドレス](#グローバルユニキャストアドレス)
      * [マルチキャスト](#マルチキャスト)
      * [エニーキャスト](#エニーキャスト)
      * [アドレス範囲](#アドレス範囲)
      * [コマンド類](#コマンド類)
         * [ping6コマンド](#ping6コマンド)
         * [ndpコマンド](#ndpコマンド)

<!--te-->

# インターネットの特徴
- Inter(相互接続された)Net(ネットワーク)
  - 全世界規模のパケット交換網
  - 自立分散型ネットワークシステム(LAN)をルータにより相互接続している．
- 基本プロトコルはTCP/IPv4(IPv6)

# パケット通信方式
- データを分割し，通信パケットにして伝送する．
  - 送信側は，データを通信パケットに分割する．
  - 受信側は，通信パケットからデータを再構成する．
- 通信パケットにはヘッダを付与して伝送する．
- ヘッダは相手の識別番号(Identifier)が設定されている．
  - TCP/IPのIPではIPアドレス．

# ネットワークシステムの階層化
- 上下関係を持つ複数のプロトコルにより構成．
  - 上位層は階層を使って，より高度な通信を行う．
- 階層間インターフェイスの標準化
  - 階層を抽象化する．
    - 階層毎に異なるプロトコルを用いることも可能である．
  - 現実的には，完全な抽象化は困難である．
- OSI参照モデル[7層モデル]との対応
  - TCP/IPは5層で定義されている．
- プロトコルスタック
  - 階層図ではプロトコルが積み重なって見える．
- 階層名とレイヤ
  - 下からレイヤnと呼ばれる．
    - レイヤ3: ネットワーク層
    - レイヤ2: データリンク層
    - レイヤ1: 物理層

# プロトコルとインターフェイス
- プロトコル(Protocol)
  - ノード間で通信を行う為の取り決め
  - 同一階層間のデータ(制御，情報)交換
- インターフェイス(Interface)
  - 上下の階層間の取り決め
  - 上下の階層間のデータ(制御，情報)交換

# 通信の分類(コネクションの型)
- コネクション(指向)型プロトコル
  - 通信する前に，論理的な通信路(仮想回線，Virtual Circuit)を設定する．
  - 通信品質，透過性，順序性が保証される．
  - TCP，電話

- コネクションレス型プロトコル
  - いきなり送信する．
  - 通信品質は保証されない(最大限努力型通信，ベストエフォート)
  - UDP，IP，イーサネット，電信，電報，郵便

# 応用層(Application Layer)
- 応用プロセス(Application Process)間で送受信されるデータに関した通信機能を制御する．
  - OSI参照モデルではさらに3層に分かれる．
- プロトコル例
  - HTTP
  - FTP
  - SMTP
  - POP3
  - IMAP4
  - telnet
  - DNS
  - NFS

# トランスポート層(Transport Layer)
- 透過的に，終端ノード間での効率の良いデータ転送を行う．
- 誤り制御，順序制御，フロー制御
- TCP(信頼性のあるコネクション型プロトコル)
- UDP(信頼性のないコネクションレス型プロトコル)

# ネットワーク層(Network Layer)
- 経路選択と中継制御を行う．
- IP(信頼性のないコネクションレス型プロトコル)

# データリンク層(Datalink Layer)
- 隣接するノード間でのデータ転送制御．
  - 同一LAN内のノード間の通信．
- 物理層と一体になって規定されることが多い．
  - イーサネットの制御(ソフトウェア)部分．
  - PPP(Point 2 Point Protocol)

# 物理層(Physical Layer)
- 電気的，物理的な信号の制御．
- イーサネットのケーブルやトポロジの規格．
- 具体例
  - イーサネットの物理(ハードウェア)部分．
  - 電話回線(アナログ，ISDN，ADSL)

# ネットワーク層 IPv4(Internet Protocol)
- ネットワーク層のプロトコル．
  - ルータ(ゲートウェイ)によりLAN間に接続する．
- 主な機能は経路選択と中継制御．
  - PCでも経路選択テーブルが必要である．

- コネクションレス型
  - ベストエフォートなので，破棄されることもある．
- アドレス(ホストを識別するユニークな番号)は32bit．
  - 割り当て可能なアドレスは枯渇している．

# IPv4アドレス
- ホストを識別する番号
  - 32bitのユニークな番号
  - インターネット内に同じIPv4アドレスを設定したホストが2台以上存在できない．
- IPv4アドレスの表記
  - 32bitを1オクテット単位に10進数で表記する．
  - 区切りは.(コロン)を使用する．
    - 172.0.0.1(localhost)
    - 1.1.1.1(Cloud Flare DNS)
    - 172.217.26.4(www.google.com)

# IPv4アドレスのビット構成
- ネットワーク部(上位ビット)
  - ネットワーク(LAN)に割り当てる．
- ホスト部(下位ビット)
  - ネットワーク(LAN)内の各ホスト(ノード)に割り当てる．
- ネットワークの規模(LAN内のホスト数)により，ネットワーク部とホスト部のビット配分を調整する．
  - アドレスのネットワーク部によりグループ(LAN)を区別する．
  - グループ化することでアドレスを集約し，経路情報を節約する．
- 割り当て可能なビット数は`2 ^ ホスト部のビット数 - 2`
  - `ネットワークのビット数=32 - ホスト部のビット数`
  - ルータ(ゲートウェイ)もホストとして数える．
  - ネットワークアドレス(ホストが000...)，ブロードキャストアドレス(ホストが111...)の分の2つを引く．

# IPv4のクラスレス(Class Less)アドレス
- ネットワーク部のビット数を明示する(CIDR表記)．
  - 例: 192.168.100.20/24 (サブネットマスクの255.255.255.0と同じ)
- サブネットマスク(Subnet Mask)指定方式
  - ネットワーク部として残すビットを1にする．

# 特別なIPv4アドレス
- ネットワーク(LAN)アドレス
  - ホスト部の全ビットが0
- 指定したネットワークへのブロードキャスト(BC)
  - ホスト部の全ビットが1
- ローカルネットワークへのブロードキャスト(BC)
  - 全ビットが1
- ループバック(LB)アドレス
  - 127.0.0.1(localhost)

# ネットワークのアドレス計算
- ネットワーク(LAN)のアドレス
  - ホストのIPv4アドレスにサブネットマスクをビット毎にAND演算する．
- ネットワークのブロードキャストアドレス
  - ホストのIPv4アドレスにサブネットマスクを反転した値をビット毎にOR演算する．

# ドメイン名(Domain Name)
- インターネット上のサイト(ホスト)の識別名のこと．
  - ホストを識別する名前．
  - FQDN(Fully Quaified Domain Name)が正式名称．
    - www.google.com.

# ドメイン名の階層構造
- ドメイン名はルートドメイン(.)からの階層構造になっている．
  - 普通は省略する．
- トップレベルドメイン(TLD: Top Level Domain)
  - ccTLD(Country code TLD)
    - 日本はjp
  - gTLD(generic TLD)
    - com, edu
- セカンドレベルドメイン(SLD Second Level Domain)
  - 日本では，co, ac, ne等．
  - gTLDには無い．
- サイトが管理するドメイン

# ドメイン，IPアドレスの変換
- 管理サーバによる変換
  - DNS(Domain Name System)サーバ
  - NISサーバ
- 表による変換
  - `/etc/hosts`
  - `\WINDOWS\system32\drivers\etc\hosts`
- 変換方法の指定(UNIX)
  - `/etc/resolv.conf`

# DNSサーバ
- 機能分散と負荷分散
  - DNSサーバはアドレス管理情報ファイルであるゾーンファイル(Zone File)を管理している．
  - 複数のDNSサーバがゾーンファイルのコピーを持っている．
    - 複数のDNSサーバを配置することで負荷分散を行う．

- DNSサーバの種類
  - プライマリDNSサーバは元となるゾーンファイルを管理している．
  - セカンダリDNSサーバはプライマリDNSサーバからゾーンファイルをコピーする．

# 名前の正引きと逆引き
- 正引き(Forward Lookup)
  - ホスト名をIPアドレスに変換する．
  - wwwのURLやtelnetのログインで使用している．
- 逆引き(Reverse Lookup)
  - IPアドレスをホスト名に変換する．

# IPデータグラムの送信
- 直接配送
  - 同一LAN内の隣接するホストに，データリンク層・物理層によりIPデータグラムを伝達する．
- 間接配送
  - 異なるLANのホストに複数のルータ(ゲートウェイ)を経由してIPデータグラムを伝達する．

# 直接配送の手順
- 通信相手の物理アドレス(MACアドレス)を解決する．
  - データリンク層・物理層がイーサネットであればARP(Address Resolution Protocol)を使用する．
- イーサネットフレームを作成し，送信する．
  - 送信先MACアドレスにはARPにより解決したMACアドレスを使用する．

# MAC(イーサネット，物理)アドレス
- MAC(Media Access Control)
  - Windowsではイーサネットアドレス，物理アドレスと言う．
  - 48bitで表現する．
- 複数の危機に同一のMACアドレスを割り当てていない．
  - 全世界でユニークな番号．
- 表記方法
  - 48bitを1オクテット単位に16進数で表記する．
  - 区切りは-(ハイフン)か:(コロン)．

# ARP(Address Resolution Protocol)
- IPデータグラムを伝達したいホストのMACアドレスを解決する．
  - 人間が作る対応表では管理が容易ではない．
    - 新しいホストの接続や，ホストの切り離しへの対応．
  - 必要な時に，ネットワークを使って解決する．
  - 解決したMACアドレスは，一定時間キャッシュされる．

# ARPの手順
- MACアドレスを解決したいホストは，ARP要求メッセージを送信する．
  - MACアドレスはブロードキャスト(1 vs all)で送信する．
- 対象のホストはARP応答メッセージを送信する．
  - MACアドレスはユニキャスト(1 vs 1)で送信する．

# 経路選択表
- 経路選択(Routing)機能
  - ネットワーク層の最も重要な機能である．
  - ルータ(ゲートウェイ)でIPデータグラムを転送する(バケツリレー)機能である．
- 経路選択表
  - 送信先IPアドレスから次に転送するルータ(ゲートウェイ)を選択する表．

# 経路選択(ルーティング)アルゴリズム
- 送信先のIPアドレスから経路エントリを探索アルゴリズムによって探索する．
  - 送信先IPアドレスに各経路エントリのネットマスクをANDして，ネットワーク宛先に一致する経路エントリを探索する．
  - 複数の経路エントリに一致した時は，ネットワーク部が最も長い経路を選択する．

- ネットワーク宛先0.0.0.0は必ず一致する．
  - デフォルトゲートウェイと呼ばれている．
    - 例えば172.25.129.45は0.0.0.0以外一致しない．
  - 経路選択表には必須の経路エントリである．
  - デフォルトゲートウェイにはインターネットに最も近いルータのIPアドレスを設定する．

# ルータ(ゲートウェイ)
- データリンク層レベルのネットワーク(イーサネット等)を相互に接続するネットワークの相互接続装置である．
- 受信したIPデータグラムに格納されている送信先IPアドレスを手掛かりに，バケツリレー方式でIPデータグラムを正しい経路に送信する．

# 間接配送の手順
- 同一LAN内から，通信相手が所属しているLANに向かう経路に接続しているルータを選択する．
  - 経路選択(ルーティング)表から探索する．
- ARPにより，ルータのMACアドレスを解決する．
- イーサネットフレームを作成し，送信する．
  - イーサネットの送信先MACアドレスは**ルータのMACアドレス**．
  - IPデータグラムの送信先IPアドレスは**通信相手のIPアドレス**．
- ルータでは，IPデータグラムを取り出し，次に転送するルータを選択する．

# IPv4ヘッダ(IPv4 Header)
- 寿命TTL(Time To Live, 8bit)
  - IPv4データグラムの寿命である．
  - 配送経路以上で永久にループすることを防止する．
  - ルータを経由する毎にデクリメントされる．
  - 0になったら，IPv4データグラムは破棄される．

```
TTLがないと，BFGDを永遠にループする．

A -> B --------       C -> E
     ^         |
     |         |
     |         v
     D <- G <- F
```

# ICMP(Internet Control Message Protocol)
- 制御・エラー通知プロトコル
- ICMPの用途
  - ホストの正常性を確認する．
  - 配送中のエラーを通知する．
  - 適切な経路情報を通知する．
  - 輻輳(ネットワークの混雑)を通知する．

# pingコマンド
- pingコマンドにICMPが実装されている．
- pingコマンドのオプション
  - TTL値

# ICMPの機能(ICMPエコー)
- 指定したホストの正常性を確認する．
  - ICMPエコー要求メッセージ
  - ICMPエコー応答メッセージ

# ICMPの機能(配送エラーの通知)
- 配送エラーを通知する．
  - 上位プロトコルが存在しない．
  - ポート番号が存在しない．
  - 送信先ネットワークインターフェースに到達不能である．

# ICMPの機能(配送エラーの通知)
- 時間切れ
  - TTLが0になった．
- 方向転換
  - 一時的に，送信元の経路情報を更新する．

# DHCP(Dynamic Host Configuration Protocol)
- 動的にIPアドレスなどを設定する．
  - ホスト
  - デフォルトゲートウェイ
  - DNSサーバのIPアドレス
  - サブネットマスク
  - etc
- 割り当て方法
  - 動的: 移動ホストや一時的に接続するホスト用．
  - 自動: IPアドレスを永久に使用するホスト用．
  - 手動: ホストに固定的にIPアドレスを設定する．
- 割り当て手順
  - クライアントとサーバ間でネゴシエーションする．
- 割り当て情報の有効期間がある．

# IPv6実用化の歴史
- IPv4からIPv6への以降がユーザやISPに全く受け入れられずに来た．
  - IPv6がIPv4に比べて顕著に優れた機能を提供するわけではない．
    - IPv6へ移行することに対するインセンティブがない．
    - ソフトウェアの変更やハードウェアの更新が必要である．
    - 移行のためにコストがかかる．
  - CIDRやプライベートアドレスがうまく機能したのですぐに移行する必要性が薄れた．
    - IPv4アドレスが永久に枯渇しないという幻想を抱かせてしまった．

# ネットワーク層 IPv6
- 広大なアドレス空間(128bit)
  - アドレス全体では`16Ei * 16Ei`個または`4Gi * 4Gi * 4Gi * 4Gi`個．
    - LAN当たりには16Ei個．
  - 多数の機器に個別にアドレスを割り当てることができる．
    - IoT(Internet of Things)
    - 各種センサや照明機器等
    - 家電製品
    - モバイル情報端末
    - etc
- IPv4ヘッダの簡略化
  - 固定長の40オクテットである．
  - 拡張ヘッダの導入．
  - ルータでの転送の高速化(ハードウェア処理)が可能になる．
- 通信品質管理とセキュリティ機能
  - ヘッダに関係するフィールドが既にある．
  - IPSecが既に規定されている(ただしオプションである)．
- アドレス割当の自動化
  - ネットワークに接続すると自動的にアドレスを設定する．
    - SLAAC(State-Less Address Auto Configuration)
  - RA(ルータ通知)，DHCPv6が既に規定されている．
- 階層化されたアドレス割当
  - IPv4の反省からアドレス割当が階層化されている．
    - SLAと呼ばれる．
   - 経路情報の集約により経路選択の負荷が軽減されている．
- [RFC 8200](https://tools.ietf.org/html/rfc8200)を参照．

# IPv6ヘッダの特徴
- IPv4ヘッダからの変更点
  - IPアドレスは128bitに拡張された．
  - 通信品質管理を高速化した．
- IPv4ヘッダからの廃止
  - ヘッダ長
    - 固定40オクテットになった．
  - データグラムの分割・再構成機能
    - 拡張ヘッダに移管した．
      - 中継点オプションヘッダ
      - 経路制御ヘッダ
      - 終点オプションヘッダ
      - 断片(分割・再構成)ヘッダ
      - 認証ヘッダ
      - 暗号化ヘッダ
  - チェックサム
    - 上位プロトコルで検査する．

```
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                       Ethernet Header                         |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                           IPv6 Header                         |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                       Extended Header                         |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                              ...                              |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                       Extended Header                         |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                                                               |
|                    Transport Layer Data                       |
|                                                               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
```

```
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|Version| Traffic Class |           Flow Label                  |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|         Payload Length        |  Next Header  |   Hop Limit   |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                                                               |
+                                                               +
|                                                               |
+                         Source Address                        +
|                                                               |
+                                                               +
|                                                               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                                                               |
+                                                               +
|                                                               |
+                      Destination Address                      +
|                                                               |
+                                                               +
|                                                               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
```
- VersionにはIPv6を表す6(4bit)が入っている．
- Traffic Classは8bitである．
- Flow Labelは20bitである．
- Payload Lengthは16bitである．
- サイズはIPv4とほぼ同じである．

# IPv6のアドレス表記方法
- 16bit(=2byte)毎，16進数，:(コロン)で区切る．
- 16進数は小文字である．
- 連続する:0000:は::に省略できる(0を記述しなくても良い)．
  - fe80::0201:02ff:fe8d:1a90
  - ただし1箇所だけである．
    - fe80::101f:0000:0000:1a90
  - 最も大きく短縮できる箇所を短縮する．
  - 左(上位ビット)から短縮する．
  - ポートを付加する際は`[]`(ブラケット)でIPを囲む．
    - `[fe80:db8::1]:22`
- プレフィックス部(ネットワーク部)を`/<n>`で表現する場合もある．
  - 2001:123:4567::1/64

# リンクローカルアドレス(LLA)
- Link Local Address
- プレフィックスはfe80::/64
- LAN内のみ有効である．
  - 全てのLANでプレフィックスが同じなので，各LANを区別できない．
  - ネットワークインターフェイス(IFID)の指定が必要である．
  - ネットワークの管理用として想定している．
- 自己完結で，自動設定可能である．

# IPv6LLAのアドレス表記方法
- リンクローカルアドレス(LLA)ではアドレスだけでIFID(network interface ID)を特定できないのでIFIDを指定する．
  - FreeBSDでは`IFID名(%<name>)`で指定する．
  - Windowsでは`IFID名(%<no>)`で指定する．

# ユニークローカルアドレス(ULA)
- Unique Local(Unicast) Address
- プレフィックスは
  - `00fd:<Global ID>:<SLA>:/64`
- サイト(組織)内のみ有効である．
  - 一般に，サイト内の通信に利用する．
  - 各LANに固有の`<SLA>`を割り当てるので，各LANを区別できる．
    - IFIDの設定は不要である．
- ルータ通知で自動設定するか，手動で設定する．

# グローバルアドレス(GUA)
- Global Unicast Address
- プレフィックスは1::/3(2進数では001)
- GRP(Grobal Routing Prefix)
  - 階層化され，経路情報を集約することで経路選択の負荷を軽減している．
- インターネット全体で有効である．
  - インターネットに接続するときに使用する．
  - 各LANに固有の`<SLA>`を割り当てるので，各LANを区別できる．
    - IFIDの指定は不要である．
- ルータ通知で自動設定するか，手動で設定する．

# インターフェースID(IFID)の生成
- 匿名アドレス方式
  - 乱数により割り当てる．
  - 24時間毎に更新する．
  - Windows Vista以降はデフォルトでこの方式である．

# EUI-64(Extended Unique ID 64 Bit)方式
- 非推奨になった，意味不明なビット列が推奨される．
- MACアドレスから生成する．

# IPv6アドレス(通信形態による分類)
- ユニキャスト(1 vs 1の通信)
  - 1台のホストに割り当てられるアドレス．
- マルチキャスト(1 vs nの通信)
  - グループに割り当てられるアドレス．
- エニーキャスト(1 vs nの通信)
  - マルチキャストと同じ，近くのホスト．

# マルチキャストアドレス
- リンクローカル・マルチキャストアドレス
  - ff02::(グループ識別子)
  - 全ノード・マルチキャストアドレス
    - ff02::1
  - 全ルータ・マルチキャストアドレス
    - ff02::2

# 特殊なIPv6アドレス
- 未定義
  - 0::0または::
- ループバック
  - 0::1または::1

# ネットワークのアドレス
- ネットワークのLANアドレス
  - IPv6では，基本的にプレフィックス(ネットワーク部)は64ビット固定である．
    - LLA -> fe80::/64，LANを区別できない．
    - ULA -> fd:`<Global ID>`:`<SLA>`::/64
    - GUA -> `<GLP>`:`<SLA>`::/64 (上位3ビットが(001))

# 経路選択(Routing)
- IPv6も，経路選択(Routing)機能と，使用する経路選択表はIPv4と同じである．
- タイトル
  - Destination: 宛先
  - Gateway: ルータのアドレス，`link#<n>`は直接配送
  - Netif: IFID

# 経路選択(ルーティング)アルゴリズム
- ネットワーク宛先 defaultは必ず一致する．
  - デフォルトゲートウェイと呼ばれている．
  - 経路選択表には必須の経路エントリである．
  - デフォルトゲートウェイにはインターネットに最も近いルータのIPアドレスを設定する．

# データリンク層のアドレスの解決
- IPv4は，ARPを使用する．
  - 要求をブロードキャストする．
  - ARPキャッシュはUNIXでは20分有効である．
- IPv6はNDP(Neighbor Discovery Protocol，近隣探索プロトコル)を使用する．
  - ICMPv6の一部である．
  - NS(近隣要請)とNA(近隣通知)を使用する．
  - `$ ndp`というコマンドが`$ arp`と同様に使える．

# NDP(Neighbor Discovery Protocol)
- ICMPv6の一部である．
  - データリンク層・物理層に依存しない．
- メッセージの種類
  - NS(近隣探索要請)メッセージ
    - IPv6アドレス重複割り当て検出にも使用している．
  - NA(近隣探索通知)メッセージ
  - RS(ルータ要請)メッセージ
  - RA(ルータ通知)メッセージ

# RS(Router Solicitation)メッセージ
- ホストが送信する．
- ホストが起動した時，自動的にRSメッセージを送信する．
- ホストはRAメッセージを受信したら，情報を記録する．

# RA(Router Advertisement)メッセージ
- ルータが送信する．
- 送信するタイミング
  - RSメッセージを受信したとに送信する．
  - 定期的(標準では600秒毎)に送信する．
- RAで通知できる情報
  - ULA，GUA等を生成するのに必要なアドレスのプレフィックス情報(Global ID，GRP，SLA)と有効時間
  - SLAACの有効性
  - DNSサーバのアドレスリスト
  - デフォルトゲートウェイのアドレス
    - RAを送ったルータのアドレス

# ステートレスアドレス自動設定
- SLAAC(State-Less Address Auto Configuration)
- 各ノードは起動時に，各スコープのアドレスを自動生成する．

# LLAの自動設定
- インターフェースIDを生成する．
  - EUI-64方式，または匿名アドレス方式等がある．
- リンクローカルアドレスを生成する．
- DAD(重複検出)を行う．

# ULA，GUAの自動設定
- 各ノードは起動時に，RS(ルータ要請)を送信し，RA(ルータ通知)を受信することによりULA等のアドレスを自動設定する．

# 応用層プログラムの識別: ポート番号
- 接続相手の応用プロセスを識別する番号．
  - 応用プロセス毎に一つしかない，ユニークな番号が必要．
  - TCP/IPではポート番号が使われている．
    - FreeBSDではlocalhost.8080
    - Windowsではlocalhost:8080

# Well-Known Port
- サーバ用のポート番号
  - インターネットの多くのコンピュータで利用されているサーバ(サービス)用の番号．
  - 0から1023
    - 21: FTP
    - 22: SSH
    - 25: SMTP
    - 80: HTTP
    - 443: HTTPS
- `$ nmap localhost -p 0-1023`で自身のWell-Known Portの状態を知ることができる．

# トランスポート層 TCP
- 信頼性のあるコネクション型プロトコル
  - 上位層に対して仮想的な通信路(VC: Virtual Circuit)を提供する．
- 信頼性を提供するための機能
  - 誤り制御(再送制御)
  - 順序制御
  - フロー制御と輻輳制御
- その他の機能
  - 全二重通信
  - バイトストリームサービス

# トランスポート層 UDP
- 信頼性のないコネクションレス型プロトコル
  - オーバーヘッドが少ない．
  - 処理効率が高く，高速である．
- UDPを使う応用層の例
  - DNS(Domain Name System)
  - NFS(Network File System)
  - 音声，動画，VoIP等のストリームデータ

# イーサネット
- データリンク層・物理層プロトコル
  - LAN(Local Area Network)用ネットワークとして開発された．
  - トポロジ(接続形態)は，バス型からスター型に移行した．
  - リピータ(帯域共有)HubからスイッチングHubに移行した．
- コネクションレス型プロトコル
  - 最前努力型(ベストエフォート)プロトコルである．
  - イーサネット・フレームが破棄されることもある．
  - 帯域共有型では衝突もある．
- 伝送速度
  - 10Mbps -> 1Gbps(10Gbps~100Gbps)まで，改良されてきた．
- LANだけでなく，WAN(Wide Area Network)にも使用されている．

# 100Base-TX
- 仕様
  - 伝送速度は，100Mbpsである．
  - 制御方式，トポロジ，ケーブル長は10Base-Tと同じであるが，ケーブルはCAT5のUTPケーブルで2対使用している．最大100m．
    - CAT5: ツイストペアケーブルの規格．
    - UTPケーブル: ツイストペアケーブル．シールド無しで電線同士を撚り線にしている．反対はSTPケーブル．
  - スイッチングHubが一般的なので接続段数に制限はない．

# 1000Base-T
- 仕様
  - 伝送速度は，1Gbpsである．
  - 制御方式は，基本的にCSMA/CDを使わない全二重方式のみ．
  - トポロジとケーブル長は，100Base-TXと同じである．
  - ケーブルはCAT5cまたはCAT6のUTPケーブルで4対使用している．最大100m．
  - スイッチングHubのみ販売されている．
  - 1000Base-T/100Base-T/10Base-Tに対応し，自動切替方式ほHubとNICが一般的に使われている．

# UTP系イーサネットの分類

| |10Base-T | 100Base-T | 1000Base-T |
|:---|:--:|:--:|:--:|
| 伝達速度 | 10Mbps | 100Mbps | 1Gbps |
| 半二重(CSMA/CD) | O | O | X |
| 全二重 | O | O | O |
| リピータHub | O | Δ | X |
| SW Hub | O | O | O |
| トポロジ | Hubを中心とするスター型 |> | >|
| ケーブルの仕様 | CAT3 | CAT5 | CAT5s/CAT6 |
| ケーブル使用対数 | 2対 | 2対 | 4対 |
| ケーブル最大長 | 100m | > | > |
| コネクタ | RJ-45 | > | > |

- `>`は左のセルとのセル結合を表す(Github Pagesではセル結合がレンダリングされない)．

# イーサネットの通信形態
- 全二重通信
  - UTPと光ファイバのみ実現可能である．
  - CSMA/CD制御方式を使用しない．
  - 送信と受信を同時にできる．
    - 見かけ上，通信速度が2倍になる．
  - 現在はこの方式が使われている．
- 半二重通信
  - 同軸ケーブル(バス型)では，この通信携帯のみ利用可能である．
  - CSMA/CD制御方式を使用する．
  - 一つのホストだけが送信できる．

# SW Hub
- データリンク層で中継する．
  - フレームを認識し，送信先MACアドレスを持つホストが接続されているポートにのみフレームを転送する．
    - 一度フレームを全て受信し，蓄積してから転送する．
  - レイヤ2スイッチとも呼ばれる．
- 特徴
  - 全二重と半二重のいずれにも対応可能である．
  - 速度の異なるセグメントも相互接続可能である．

# Wi-Fi(無線LAN)
- Wi-Fi Allianceで認定された機器には，Wi-Fiロゴの使用が許可される．
- 正式な規格名はIEEE802.11であり，方式によりIEEE802.11a等の名称がつけられている．
  - 2019年からWi-Fi`<n>`と表記することになる．
    - 11n  -> Wi-Fi4
    - 11ac -> Wi-Fi5
- 親機(AP)と複数の子機間で無線による通信を行う．
  - 無線LANに使われる無線方式は省電力無線方式のため無線局の免許は不要である．

# 周波数帯域(2.4GHz帯)
- IEEE802.11/b/g/n/axで使用している．
- 帯域幅20MHz，14チャネル
  - 各チャネルの周波数帯が重なっており，干渉なしに通信できるのは実質的に3チャネルである．
  - 使用可能なチャネル数が少なく，混信が多い．
  - 屋内，屋外とも通信可能である．
  - bluetooth等の無線システム，電子レンジも同じ周波数帯を使用しているため干渉が多い．
  - 壁等の障害物があっても遠くまで届きやすい．

# 周波数帯域(5GHz帯)
- IEEE802.11/a/n/ac/axで使用している．
- 帯域幅20MHz，19チャネル
  - チャネルの周波数帯が重なっておらず，前チャネルの干渉が無く，使用できるチャネル数が多い．
  - 帯域のグループはW52，W53，W56がある．
    - W52とW53は**屋内のみ使用可能**である．
  - 他の機器から干渉を受ける可能性が2.4GHz帯より低い．
  - 壁等の障害物があると電波が届きにくくなる．

# Wi-Fi(無線LAN)の方式

| 方式 | Wi-Fi | 規格年 | 周波数帯 | 公称速度 | チャネルボンディング | MIMO | 多重化 |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| IEEE802.11a | Wi-Fi1 | 1999 | 5G | 54Mbps | なし | なし | 6bit |
| IEEE802.11b | Wi-Fi2 | 1999 | 2.4G | 11Mbps | なし | なし | 6bit |
| IEEE802.11g | Wi-Fi3 | 2003 | 2.4G | 54Mbps | なし | なし | 6bit |
| IEEE802.11n | Wi-Fi4 | 2009 | 2.4/5G | 150Mbps~600Mbps | x2 | 4x4 | 8bit |
| IEEE802.11ac | Wi-Fi5 | 2013 | 5G | 433Mbps~1.7Gbps | x8 | 8x8 MU-MIMO | 8bit |
| IEEE802.11ax | Wi-Fi6 | 2019 | 2.4/5G | 433Mbps~4.8Gbps | x8 | 8x8 MU-MIMO | 10bit |

- `>`は左のセルとのセル結合を表す(Github Pagesではセル結合がレンダリングされない)．

# IPv6のまとめ

## IPv6のフィールド分割によるアドレス構造

IPv6のIPを簡単に分割する．

```
                               128
|         n         |   64-n    |             64                |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|   User Network    |    SLA    |            IFID               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
```

次に，用途によって以下のように分けられる．

- ユニキャスト(1 vs 1の通信)
  - ユニークローカル・ユニキャストアドレス
    - いわゆるIPv4のプライベートIPアドレスに相当する．
    - サイト(組織)内で使用される．
  - リンクローカル・ユニキャストアドレス
    - いわゆるIPv4のリンクローカルアドレスに相当する．
    - 同一ネットワーク内に接続されているアドレス．
  - グローバル・ユニキャストアドレス
    - いわゆるIPv4のグローバルIPアドレスに相当する．
- マルチキャスト(1 vs nの通信)
- エニーキャスト(1 vs nの通信)
  - IPv4にはない機能である．


## ユニキャストのフィールド

### ユニークローカル・ユニキャストアドレス
- feは16進数である．
- LはグローバルIDの使用方法フラグ．
- Global IDはランダム値．
- SLAはサイトの階層を識別する識別子．
- IFIDはいわゆるホストアドレスである．

```
                               128
| 7 |1|     40      |    16     |             64                |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|fc +L|  Global ID  |    SLA    |            IFID               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

```

### リンクローカル・ユニキャストアドレス
- IFID以外は16進数である．
- IFIDはいわゆるホストアドレスである．

```
                               128
|  16   |      32       |  16   |             64                |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
| fe80  |   0000 0000   | 0000  |            IFID               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

```

### グローバル・ユニキャストアドレス
- 001は16進数である．
- GRP(Global Routing Prefix)はサイトに割り当てられたアドレス範囲を識別する．
- SLAはサイトの階層を識別する識別子．
- IFIDはいわゆるホストアドレスである．

```
                               128
| 3 |        45         |  16   |             64                |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|001|       GRP         | SLA   |            IFID               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

```

## マルチキャスト
- ffは16進数である．
- フラグフィールドはマルチキャストアドレスが一時的か恒久かを区別するフラグ．
- スコープフィールドは範囲を表すフラグ．
- Group IDはアドレス管理機関が管理するID(個人向けでない).

```
                               126byte
|8b |4|4|                                                       |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|ff | | |                      Group ID                         |
+-+-+++++-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
     | |
     |_|_ フラグフィールド
       |
       |_ スコープフィールド

```

## エニーキャスト
- 構造がグローバル・ユニキャストアドレスと同じであり，見分けがつかない．
- 同じアドレスを割り当てられた複数の受信側のホストがそのアドレスがエニーキャストであると認識する必要がある．

## アドレス範囲

|名称|アドレス範囲|
|:---|---:|
|ループバック|`::1/128`|
|ユニークローカルキャストアドレス|`fd00::/7`(L=1, fc+1=fd)|
|リンクローカルキャストアドレス|`fe80::/10`|
|グローバルユニキャストアドレス|その他|
|マルチキャストアドレス|`fe00::/8`|

## コマンド類

### ping6コマンド
- `$ ping -6`と同じ動作．

### ndpコマンド
- `$ arp`と同様の動作．

[戻る](#ネットワーク層-ipv6)
