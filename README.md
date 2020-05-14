# <img src="app/assets/images/logo.png" width="100" height="100"> ながの CAKE 

長野県にある小さなな洋菓子店「ながのCAKE」の商品を通販するためのECサイト  
元々近隣住民が顧客だったが、昨年始めたInstagramが人気となり、全国から注文が来るようになった。  
InstagramのDMやメールで通販の注文を受けていたが、情報管理が煩雑になってきたため、管理機能を含んだ通販サイトを開設しようと思い至った。(コロナに負けない優良店舗) 

# 使い方
_インストール方法_  
    $ git clone git@github.com:DMM-WEBCAMP-Avengers/nagano_cake.git(SSH)  
        or $ git clone https://github.com/DMM-WEBCAMP-Avengers/nagano_cake.git (HTTPS) 
    $ cd nagano-cake  
    $ bundle install  
    $ rails db:migrate  
    $ rails db:seed  
    $ rails s -b 0.0.0.0  

_テスト方法_  
ターミナルで上記の作業を行った後、  
[ローカルサーバー](http://localhost:3000)にアクセスしてご覧ください。  

- 管理者用アカウント  
メールアドレス：admin@example.com  
パスワード：password  
を入力してログインしてください。  

- 顧客用アカウント
メールアドレス：example0@gmail.com  
パスワード：password  
を入力してログインしてください。  
（登録画面にて新規登録も可能です。）  


# 実装機能

| 機能名 | 説明 |非ログイン時利用可否|
|---|---|---|
|顧客|||
| 1ログイン機能 |・メールアドレス、パスワードでログインできる。 ・ログイン時のみ利用できる機能が利用できるようになる。|○|
|2ログアウト機能|・ログインしている状態からログアウト状態にする。 ・ログイン時のみ利用できる機能が利用できなくなる。|×|
|3商品一覧表示機能|・商品を一覧表示する。 ・検索結果を表示する場合は、検索条件に当てはまる商品のみ一覧表示する。|○|
|4商品詳細情報表示機能|・商品一覧画面で選択した商品の詳細情報を表示する。 ・カート追加機能が表示されている。|○|
|5カート追加機能|・カートに商品を追加することができる。|×|
|6カート一覧機能|・カートの中身を一覧表示することができる。|×|
|7カート編集機能|・カートの中身の個数を編集したり、削除したりすることができる。|×|
|8注文機能|・カートの中身の購入をすることができる。 ・支払方法や発送先を設定することができる。|×|
|9会員情報編集機能|・登録している情報を編集することができる。|×|
|10退会機能|・退会手続きをすることができる。|×|
|11配送先追加・編集機能|・登録している配送先を一覧で確認することができる。 ・配送先の新規追加・修正・削除をすることができる。|×|
|12注文履歴一覧表示機能|・過去の注文概要を一覧で確認することができる。|×|
|13注文履歴詳細表示機能|・注文の詳細(注文商品や個数など)を確認することができる。|×|  

| 機能名 | 説明 |非ログイン時利用可否|
|---|---|---|
|管理者|||
|1ログイン機能|・メールアドレス、パスワードでログインできる。 ・ログイン時のみ利用できる機能が利用できるようになる。|○|
|2ログアウト機能|・ログインしている状態からログアウト状態にする。 ・ログイン時のみ利用できる機能が利用できなくなる。|×|
|3注文履歴一覧表示機能|・過去の注文概要を一覧で確認することができる。|×|
|4注文履歴詳細表示機能|・注文の詳細(注文商品や個数など)を確認することができる。 ・注文ステータス、製作ステータスを変更することができる|×|
|5顧客一覧表示機能|・顧客情報を一覧で確認することができる。|×|
|6顧客詳細情報表示機能|・顧客の詳細情報を確認することができる。 ・顧客のステータス(有効/退会)を切り替えることができる。|×|
|7商品一覧表示機能|・登録商品を一覧で確認することができる。|×|
|8商品詳細情報表示機能|・商品の詳細情報を確認することができる。|×|
|9商品情報変更機能|・商品の登録情報を変更することができる。 ・販売ステータスを変更することができる。|×|
|10ジャンル設定機能|・ジャンルの追加・変更・ステータス切り替えを行うことができる。|×|

# 開発環境
- Vagrant
- Ruby 2.5.7
    - Rails 5.2.4.2
- Gems 
    - devise
    - refile
    - refile-mini_magick
    - bootstrap-sass 3.3.6
    - jquery-rails
    - kaminari 1.1.1
    - faker
    - rails-i18n
##### DMM WEBCAMP 2ヶ月目課題製作グループ アベンジャーズ(いっとう とし ゆう たっけ 計4名)  