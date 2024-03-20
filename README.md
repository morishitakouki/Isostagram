## <div id="top">使用技術一覧</div>

<!-- シールド一覧 -->
<p style="display: inline">
  <!-- フロントエンドのフレームワーク一覧 -->
  <img src="https://img.shields.io/badge/-Node.js-000000.svg?logo=node.js&style=for-the-badge">
  <img src="https://img.shields.io/badge/-React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB">
  <!-- バックエンドのフレームワーク一覧 -->
 <img src="https://img.shields.io/badge/-Rails-CC0000.svg?logo=rails&style=for-the-badge">

  <!-- バックエンドの言語一覧 -->
<img src="https://img.shields.io/badge/-Ruby-CC342D.svg?logo=ruby&style=for-the-badge">
  <!-- ミドルウェア一覧 -->
<img src="https://img.shields.io/badge/-MySQL-4479A1.svg?logo=mysql&style=for-the-badge&logoColor=white">
<img src="https://img.shields.io/badge/-Bootstrap-563D7C.svg?logo=bootstrap&style=for-the-badge">

  <!-- インフラ一覧 -->
  <img src="https://img.shields.io/badge/-Docker-1488C6.svg?logo=docker&style=for-the-badge">
<img src="https://img.shields.io/badge/-Heroku-430098.svg?logo=heroku&style=for-the-badge">
  <img src="https://img.shields.io/badge/-Amazon%20aws-232F3E.svg?logo=amazon-aws&style=for-the-badge">
</p>

## 目次

1. [アプリ名](#Isostagram)
2. [環境](#環境)
3. [ER図](#ER図)
4. [使用技術詳細](#使用技術詳細)
5. [アプリ機能](#アプリ機能)
6. [ローカルでの起動方法](#ローカルでの起動方法)
7. [お問い合わせ](#お問い合わせ) 

<br />

## Isostagram


[![Image from Gyazo](https://i.gyazo.com/73b0c6a1d0c8131b9fb3a075ba122083.png)](https://gyazo.com/73b0c6a1d0c8131b9fb3a075ba122083)

 **Github** : https://github.com/morishitakouki/Isostagram/tree/main
**url** : https://rails-react-frontend-blog-e49b147a0c56.herokuapp.com/

## アプリの概要
バックエンドにrailsとフロントエンドにreactを使ったblogアプリを作りました。




  <p align="left">
    <br />
    <!-- プロジェクト詳細にBacklogのWikiのリンク -->
    <a href="Backlogのwikiリンク"><strong>プロジェクト詳細 »</strong></a>
    <br />
    <br />



## 環境

<!-- 言語、フレームワーク、ミドルウェア、インフラの一覧とバージョンを記載 -->

| 言語・フレームワーク  | バージョン |
| --------------------- | ---------- |
| Ruby                  | 3.3.0    　|
| Ruby on Rails         |  7.0.8.1   |
| MySQL                 | 8.0        |
| Node.js               | 20.11.1   　|
| React                 | 18.2.0     |



その他のバージョンはGemfileとpackage.json を参照してください。





## ER図

[![Image from Gyazo](https://i.gyazo.com/0691c96afefeba035575610fbe239859.png)](https://gyazo.com/0691c96afefeba035575610fbe239859)

<p align="right">(<a href="#Isostagram">トップへ</a>)</p>

## 使用技術詳細

### Backend

- ``devise / devise_token_auth``を使用したトークン認証機能
- ``carrierwave``を用い``Amazon S3``に画像を保存する投稿機能

### Frontend

- **コード解析**: ESLint
- **CSSフレームワーク**: react-bootstrap 
- **主要パッケージ**: Axios / react-router-dom / @mui/material / styled-components / react-hook-form /  react-bootstrap, bootstrap 

### Infrastructure, Development Environment

- **開発プラットフォーム** : Docker 
- **インフラ** :  AWS( S3) / Heroku *デプロイ
<br />


## アプリ機能


#### トップページ / ログイン

railsAPIから返されたトークン認証情報をローカルストレージに保存しています。
React hooksのuseContextを使いどのページでもログインしてるか否かを判別しログインしていなければ新規登録とログイン画面以外にアクセスできないようにしています。

<a href="https://gyazo.com/7dce9e2267ec7c32065eb5440aebcd09"><img src="https://i.gyazo.com/7dce9e2267ec7c32065eb5440aebcd09.gif" alt="Image from Gyazo" width="1000"/></a>

<a href="https://gyazo.com/8f4671d44f1944bf3e28232081034e0d"><img src="https://i.gyazo.com/8f4671d44f1944bf3e28232081034e0d.gif" alt="Image from Gyazo" width="1000"/></a>
<br />

### 新規登録
react-hook-formを使いバリデーションを実装しました。

<a href="https://gyazo.com/a3048fe6796962387460213ce594abb1"><img src="https://i.gyazo.com/a3048fe6796962387460213ce594abb1.gif" alt="Image from Gyazo" width="1000"/></a>
<br />

### ブログ投稿

<a href="https://gyazo.com/792a19d68cf8460265fa7aad3edee6b5"><img src="https://i.gyazo.com/792a19d68cf8460265fa7aad3edee6b5.gif" alt="Image from Gyazo" width="1000"/></a>

<br />

### ブックマーク機能

<a href="https://gyazo.com/792a19d68cf8460265fa7aad3edee6b5"><img src="https://i.gyazo.com/792a19d68cf8460265fa7aad3edee6b5.gif" alt="Image from Gyazo" width="1000"/></a>

### 編集機能

<a href="https://gyazo.com/f365e520ab6c1f8166ebf8e6b4a972e0"><img src="https://i.gyazo.com/f365e520ab6c1f8166ebf8e6b4a972e0.gif" alt="Image from Gyazo" width="1000"/></a>
<br /> 

### 削除機能

<a href="https://gyazo.com/7baa34d4d51b440bf3c8c2f7f0e1e3cc"><img src="https://i.gyazo.com/7baa34d4d51b440bf3c8c2f7f0e1e3cc.gif" alt="Image from Gyazo" width="1000"/></a>
<br /> 

### ログアウト

<a href="https://gyazo.com/11bfce8c34ff425ee8c2497c3153da62"><img src="https://i.gyazo.com/11bfce8c34ff425ee8c2497c3153da62.gif" alt="Image from Gyazo" width="1000"/></a>
<br /> 

## ローカルでの起動方法
1.   forkボタンをクリック
2. ``$ git clone git@github.com:{your repository name}/Isostagram.git``
3. ``frontend/Dockerfile``の``CMD ["serve", "-s", "build"]``をコメントアウト
4. ``$ cd Isostagram ``
5. ``$ docker compose build ``
6. ``$ docker compose up -d``
7. ``$ docker compose exec api bash``
8. ``$ api# rails db:migrate ``
9. ``$ docker compose exec front bash``
10. ``$ front# npm i``
11. ``$ front# npm run dev``

本番環境にpushする時は``CMD ["serve", "-s", "build"]``のコメントアウトを解除してください。

## お問い合わせ

**gmail** : ``morimori.plane.0615@gmail.com``



