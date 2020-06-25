・アプリ名

Todoリスト

・概要

リストの作成、編集、削除、リストチェック

・本番環境

https://vast-inlet-49583.herokuapp.com/


・制作背景

Trelloのような便利なTodoアプリを作成してみたかった。

・DEMO

メールアドレス：test@gmail.com

パスワード：123456

https://gyazo.com/5843107b39126553971df3fb1f3a1d29

https://gyazo.com/c8fa22b226474945e7da50090e120746

https://gyazo.com/dd75b5067f928e0e7c7edbbfe18c313f

　

・工夫したポイント
リストの中にカードメモを表示できるようにした。
リストとカードに編集機能、削除機能を実装した。


・使用技術

HTML/CSS,Ruby on Rails,JavaScript, MySQL, Git

・課題や今後実装したい機能

リスト移動

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
