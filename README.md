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
|id|integer|null: false｜
|email|integer|null: false｜
|username|string|null: false｜


has_many messages, through: image


massegesテーブル
||Column|Type|Options|
|------|----|-------|
|messages|text|
|image|string|
|group_id|interger|null: false, foreign_key: true|
|user_id|interger|null: false, foreign_key: true|


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
