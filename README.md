# テーブル設計

##　usersテーブル

| Column     | Type   | Option   |
| ---------- | ------ | -------- |
| email      | string | NOT NULL |
| password   | string | NOT NULL |
| name       | string | NOT NULL |
| profile    | text   | NOT NULL |
| occupation | text   | NOT NULL |
| position   | text   | NOT NUll |

## commentsテーブル

| Column     | Type       | Option   |
| ---------- | ---------- | -------- |
| text       | text       | NOT NULL |
| user       | references | -------- |
| prototype  | references | -------- |

## prototypeテーブル

| Column     | Type       | Option   |
| ---------- | ---------- | -------- |
| title      | string     | NOT NULL |
| catch_copy | string     | NOT NULL |
| concept    | string     | NOT NULL |
| user       | references | -------- |