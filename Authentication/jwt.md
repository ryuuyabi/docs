## JWT(JSON Web Token)

JWTとはクライアントに受け渡すJSONを暗号(ハッシュ化)する。

### JWTについて
JWTは主に `header` `payload` `signature` の3つの要素で構成されている。
JWTの構成は `header.payload.signature`です。

### JWTの流れ
1. ユーザがクライアント画面にアクセス
2. クライアントはローカルストレージに保存されているアクセストークン(JWT)が有効かサーバーに送信して検証する
3. 有効の場合はログイン認証、無効の場合はログイン画面に遷移する

参考URL : https://assets.ctfassets.net/2ntc334xpx65/5HColfm15cUhMmDQnupNzd/30d5913d94e79462043f6d8e3f557351/jwt-handbook-jp.pdf
