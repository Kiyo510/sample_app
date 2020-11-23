## プログラミングチームをつくろう！の概要
「プログラミングチームを作ろう！」、略して「プロつく！」というサービスを今年の11月初旬にリリースし、運用しております。
このサービスはプログラミングの勉強仲間や、起業仲間を探している人同士をマッチングさせるサービスになります。
## 採用担当者様へ
 ログインしなくてもトップページの下部からユーザー詳細画面や記事詳細画面は閲覧できる仕様になっております。<br>
 採用担当者様専用アカウントも用意しておりますので、必要であればこちらのアカウントを使ってログインしていただけますと幸いです。（実運用しているサービスなのでゲストログイン機能はないです。申し訳ありません。）
 
 **Eメール: guest@guest.com<br>**
 **パスワード: guest123**

## URL
https://protuku.com
  
## サービス構成図
![protuku_app_architecture-Page-1](https://user-images.githubusercontent.com/62272140/99930572-e24c6800-2d94-11eb-8576-01966af2e4af.jpg)
  
## 主な機能
### ユーザー関連
- ユーザー登録機能
- マイページ、編集、削除（退会）機能
- 自分の投稿履歴一覧表示機能
- 投稿ストック（お気に入り）履歴一覧表示機能
- アカウント有効化機能
- パスワードリセット機能
- ログイン機能
- Twitterログイン機能
- SNSシェア（Twitter)機能
- ダイレクトメッセージ機能
- ダイレクトメッセージ一覧表示機能
- 投稿ストック（お気に入り）機能
- メッセージ＆お気に入り受信時の通知機能
- プロフィール画像アップロード機能

### 投稿関連
- 新規投稿機能
- Markdownリアルタイムプレビュー機能
- 投稿検索機能
- 投稿一覧の表示、 詳細、編集、削除機能
- 投稿へのタグ付け機能
- 投稿タグによる絞り込み検索機能
- 投稿画像アップロード機能
- 各種ページネーション機能

### その他
- Google アナリティクス
- 単体・統合テスト機能(RSpec）
- レスポンシブ対応

## 使用技術
- 言語/フレームワーク
  - Ruby2.7.1/Rails6.0
- DB
  - MySQL
- 開発環境
  - Docker
  - nginx
- 本番環境
  - ALB
  - ACM
  - CloudWatch
  - ECS
  - ECR
  - EC2
  - RDS
  - Route53
  - S3
  - VPC
- CI/CD
  - CircleCI(gitへのpush時にRSpec、Rubocopも実行）
  
## 今後やっていきたいこと
- Google アドセンスを設置したり、新機能を追加するなどして、収益化に挑戦してみる。
- フロントにVue.jsなどを導入し、より良いUI/UXを提供する。
- Terraformなどでインフラをコードで管理できるようにする。
- 複雑な処理はサービスクラスを作る、行数の多いコントローラーは分割するなどして、fatなモデルやコントローラーを解消し、コードの見通しを良くする。
