
テーブル構造
usersテーブル
email (string型, NOT NULL, ユニーク制約): ユーザーのメールアドレス
encrypted_password (string型, NOT NULL): パスワードの暗号化された値
name (string型, NOT NULL): ユーザーの名前
profile (text型, NOT NULL): ユーザーのプロフィール情報
OCCUPATION (text型, NOT NULL): ユーザーの職業情報

commentsテーブル
content (text型, NOT NULL): コメントの内容
prototype_id (reference型, NOT NULL, 外部キー): コメントが紐づくプロトタイプのID
user_id (reference型, NOT NULL): コメントを投稿したユーザーのID

prototypesテーブル
title (string型, NOT NULL): プロトタイプのタイトル
concept (text型, NOT NULL): プロトタイプの概念やアイデア
user_id (reference型, NOT NULL, 外部キー): プロトタイプを作成したユーザーのID
