・アプリ名

Todoリスト

・概要

リストの作成、編集、削除、リストチェック

・本番環境



・制作背景

Trelloのような便利なTodoアプリを作成してみたかった。

・DEMO

　

・工夫したポイント



・使用技術

HTML/CSS,Ruby on Rails,JavaScript, MySQL, Git

・課題や今後実装したい機能

ログイン、ログアウト、リスト詳細、カードの作成

・DB設計
## usersテーブル
|Column|Type|Options|
|------|----|-------|
|email|string|null: false|
|password|string|null: false|
|nickname|string|null: false|
### Association
- has_many :tasks


## listテーブル
|Column|Type|Options|
|------|----|-------|
|text|text||
|user_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :user
