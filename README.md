# README


# BookValuer
### Heroku:
### AWS:



## 概要
あなたが本にお金で価値をつける。
そして、それを可視化するサービス。

## コンセプト
光元さんの価格自由にインスパイアされたサービス
本サービスはお金を一切支払いません。
支払うのは、お客様だけです。
前提、皆のgiveが可視化されれば世界は良い方向に傾きそう。

## バージョン
- Ruby
- Rails

## 機能一覧
- [ ] Book登録機能
  - [ ] BookのCRUD機能（一覧、作成、詳細、更新、削除）
  - [ ] 確認画面機能（新規投稿のみ）


  - [ ] Bookの’あとで見る’機能（一覧、追加、削除）
    - [ ] あとで見る機能の一覧表示機能
    - [ ] あとで見るリストの編集機能（追加、削除）

- [ ] ユーザ機能
  - [ ] ユーザ機能（作成、詳細、更新）

- [ ] ログイン機能  

- [ ] レビュー機能（金額を支払った時のみ、可能になる）

- [ ] フォロー機能とフォロワー機能
  - [ ] フォローとフォロワー機能（一覧表示、追加、削除）


- [ ] ユーザ管理機能（RailsAdmin）
  - [ ] ユーザのCURD機能（作成、詳細、更新、削除）
  - [ ] ユーザ削除機能
    - [ ] ユーザの編集と削除は作成したユーザと管理者のみ実行可能

- [ ] ランキング機能  (ソート機能)
- [ ] ラベル機能
- [ ] 簡易版ゲストログイン機能
- [ ] Book検索機能(Gem:Runsack)
- [ ] 画像アップロード機能(Gem:carrierwave)
- [ ] ページネーション機能(Gem:Kaminari)
- [ ] ログイン機能（Gem:Devise）



## カタログ設計
詳細は[こちら](#)をご覧ください。

## テーブル定義
詳細は[こちら](#)をご覧ください。

## ER図
詳細は[こちら](#)をご覧ください。

## 画面遷移図
詳細は[こちら](#)をご覧ください。

## 画面ワイヤーフレーム
詳細は[こちら](#)をご覧ください。

# 使用技術
- ログイン機能
  - devise
  - omniauth
  - omniauth-google-oauth2（Herokuのみ）
- 管理者機能
  - rails_admin
- 権限管理
  - cancancan
- 画像編集機能
  - carrierwave
  <!-- - mini_magick -->
- 検索機能
  - ransack
- ページネーション
  - kamminari
- デバッグ
  - better_errors
  - binding_of_caller
  - pry-rails
- テスト
  - rspec-rails
  - spring
  - spring-commands-rspec
  - factory_bot_rails
  - capybara
  - selenium-webdriver
  - database_cleaner
  - launchy
  - faker
  - gimei
- デザイン
  - bootstrap
  - kaminari-bootstrap
  <!-- - Font Awesome -->
- 辞書機能
  - i18n


## How to Start

```
1. $ git clone https://github.com/KakeruYamamoto/BookValuer.git
2. $ cd BookValuer
3. $ bundle install
4. $ yarn install
5. $ rails db:create
6. $ rails db:migrate
<!-- 7.  #config/initializers/locale.rb内の"I18n"の二行をコメントアウト（8.のコマンド終了後、戻す） -->
8. $ rails db:seed
9. $ bundle exec rspec
10.  rails s  
```
