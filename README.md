# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

userテーブル
|Column|Type|Options|
|------|----|-------|
|email|integer|
|username|varchar255|

belongs_to group
has_many masseges

massegesテーブル
||Column|Type|Options|
|------|----|-------|
|masseges|text|
|image|string|
|group_id|interger|
|user_id|interger|

belongs_to user

groups_usersテーブル

|Column|Type|Options|
|------|----|-------|
|user_id|integer|null: false, foreign_key: true|
|group_id|integer|null: false, foreign_key: true|

 Association
- belongs_to :group
- belongs_to :user

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
