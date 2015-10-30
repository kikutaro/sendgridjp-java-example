# sendgridjp-java-example

本コードは[SendGrid公式Javaライブラリ](https://github.com/sendgrid/sendgrid-java)の利用サンプルです。

## 使い方

```bash
git clone http://github.com/sendgridjp/sendgridjp-java-example.git
cd sendgridjp-java-example
cp .env.example .env
# .envファイルを編集してください
gradle build
./run.sh
```
`{"message":"success"}`と表示されたら送信成功です。

## .envファイルの編集
.envファイルは以下のようになっています。

```bash
API_KEY=api_key
TOS=you@youremail.com,friend1@friendemail.com,friend2@friendemail.com
FROM=you@youremail.com
```
API_KEY:SendGridの[API Key](https://sendgrid.kke.co.jp/docs/User_Manual_JP/Settings/api_keys.html)を指定してください。  
TOS:宛先をカンマ区切りで指定してください。  
FROM:送信元アドレスを指定してください。  
