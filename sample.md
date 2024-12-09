# ColorMe説明文
### 参照
[コンバージョンタグの設定方法について](https://help.shop-pro.jp/hc/ja/articles/360062486394-%E3%82%B3%E3%83%B3%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E3%82%BF%E3%82%B0%E3%81%AE%E8%A8%AD%E5%AE%9A%E6%96%B9%E6%B3%95%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6)  
[コンバージョンに関わる独自タグの設定](https://help.shop-pro.jp/hc/ja/articles/360062483674-%E3%82%B3%E3%83%B3%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E3%81%AB%E9%96%A2%E3%82%8F%E3%82%8B%E7%8B%AC%E8%87%AA%E3%82%BF%E3%82%B0%E3%81%AE%E8%A8%AD%E5%AE%9A)  
[GA4 eコマース設定の方法](https://help.shop-pro.jp/hc/ja/articles/360062480954-Google-Analytics-GA4-e%E3%82%B3%E3%83%9E%E3%83%BC%E3%82%B9%E8%A8%AD%E5%AE%9A%E3%81%AE%E6%96%B9%E6%B3%95)  
[GTMは利用できますか？](https://help.shop-pro.jp/hc/ja/articles/360051831593-Google%E3%82%BF%E3%82%B0%E3%83%9E%E3%83%8D%E3%83%BC%E3%82%B8%E3%83%A3%E3%83%BC-gtm-%E3%81%AF%E5%88%A9%E7%94%A8%E3%81%A7%E3%81%8D%E3%81%BE%E3%81%99%E3%81%8B-)  

### How to call Colorme object?
`parentWin.Colorme`
![307680580-f6ab8f95-cd86-43ee-8bf9-72891ec413e5](https://github.com/user-attachments/assets/30d793b7-99d6-47b3-8c30-fde2463367dc)  
<br></br>
### GTAG購入拡張CV自動取得はできるか？
- できるよう...?

### eコマースは自動で設定できるか？
- できます！！  
- 公式資料：[GA4 eコマース設定の方法](https://help.shop-pro.jp/hc/ja/articles/360062480954-Google-Analytics-GA4-e%E3%82%B3%E3%83%9E%E3%83%BC%E3%82%B9%E8%A8%AD%E5%AE%9A%E3%81%AE%E6%96%B9%E6%B3%95)

### GTMは使える？
- 条件：
  1. プレミアムプランプラン
  2. アプリを購入（アプリ名：[タグ管理 for GTM](https://app.shop-pro.jp/apps/633)）
- 参照：公式資料：[GTMは利用できますか？](https://help.shop-pro.jp/hc/ja/articles/360051831593-Google%E3%82%BF%E3%82%B0%E3%83%9E%E3%83%8D%E3%83%BC%E3%82%B8%E3%83%A3%E3%83%BC-gtm-%E3%81%AF%E5%88%A9%E7%94%A8%E3%81%A7%E3%81%8D%E3%81%BE%E3%81%99%E3%81%8B-)   
 > タグ管理 for GTMは、**プレミアムプラン**を契約されているショップオーナーさまのみご利用いただくことが可能です。

<br></br>
## グローバルサイトタグ / GTMの貼り付ける場所
- ２つの場所に設定していただく
  
#### 場所１：購入ページ以外、ウェブサイト全体に反映する場所  
- 集客 ＞ [検索エンジン対策](http://admin.shop-pro.jp/?mode=design_base) > 共通 > 一番下「headタグ内フリースペース設定」のすべての項目
<br></br>
![306837108-c23c172f-63e3-42a4-8020-2cd416089ca2](https://github.com/user-attachments/assets/03c30376-65df-4b0c-b3a4-dd9be1e07d04)  

#### 場所２：購入ページだけに反映する場所  
- ツール > コンバージョンタグ (らしい)
- または下記リンクをお客様に送り、クリックしたら該当する画面が開く
  - http://admin.shop-pro.jp/?mode=conversion_tag_edt
- 基本的に的に `body` に貼り付ける
- [公式サイト](https://help.shop-pro.jp/hc/ja/articles/360062486394-%E3%82%B3%E3%83%B3%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E3%82%BF%E3%82%B0%E3%81%AE%E8%A8%AD%E5%AE%9A%E6%96%B9%E6%B3%95%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6)からは、`head`に貼り付けると反映されない場合があるとの記載があるから（下記画像を参照）
<br></br>
![306861643-97f44887-fca5-4fc2-b7f4-a222c2859d4c](https://github.com/user-attachments/assets/fe60abdd-21ac-4ffd-a17e-3a3c5ecdb374)  
<br></br>
  
## イベントスニペットの貼り付ける場所
### 設置場所（イベントスニペット）
- 上記「場所２」と同様：ツール > コンバージョンタグ
- または下記リンクをお客様に送り、クリックしたら該当する画面が開く
  - http://admin.shop-pro.jp/?mode=conversion_tag_edt
- グローバルサイトタグの**下**に貼り付ける
  
### 「購入 + 動的値」の場合
- まずはグローバルサイトタグが下記ページにあることを確認
  - ①購入完了ページ、と
  - ②完了ページ以外全ページ
- あれば、下記イベントスニペットを貼り付ける

```html
<!-- Event snippet for 購入完了 conversion page -->
<script>
gtag('event', 'conversion', {
'send_to': 'AW-999/XXX',
'value': <{$order_price}>,
'currency': 'JPY',
'transaction_id': <{$order_no}>
});
</script>
```
<br></br>
### 「購入 + 動的値 + 拡張」の場合
- ❗要確認 ❗
- - まずは購入完了ページの<head>〜</head>に設置（グローバルサイトタグの下に）
- ColorMe公式サイトによると、headタグ内で発火できない場合がある
  - その場合は、  <body>〜</body>設置（グローバルサイトタグも）
```html
<script>
var parentWin = window.parent;
var email_data = parentWin.Colorme.customer.email;
var phone_data = '81' + parentWin.Colorme.customer.phone_number.replace(/^0/, "");

gtag('set','user_data', {
'email': email_data,
'phone_number': phone_data
});
</script>
<!-- Event snippet for 購入完了 conversion page -->
<script>
gtag('event', 'conversion', {
'send_to': 'AW-999/XXX',
'value': <{$order_price}>,
'currency': 'JPY',
'transaction_id': <{$order_no}>
});
</script>
```
