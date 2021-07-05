
# 次にやりたいこと・作りたいもの

プライベートで達成したい目標・やりたいことを管理

## 年間目標

### 2021年度

- [ ] AWS認定試験11種合格
  - [x] DVA
  - [x] SAP
  - [x] DOP
  - [x] SCS
  - [x] DS
  - [ ] ANS
  - [ ] DAS
  - [ ] MLS
- [ ] CKA合格

## AWS関連

AWS11冠を目指しながら学習する中で作ってみたいと思ったものをまとめ。

作成したらリポジトリのリンクを随時貼っていきます。

- EC2あれこれ
  - [x] 平日の深夜や土日に特定のタグが付与されたEC2インスタンスを停止する
    - CloudWatchEvents + Lambdaでスケジューリング実行
    - [やってみたリポジトリ](https://github.com/bun913/lamdba_ec2_stop)
  - [ ] 上に関連して特定のタグが付与されたEC2インスタンスを毎朝起動する
    - CloudWatchEvents + Lambdaでスケジューリング実行
- セキュリティ・コンプライアンス
  - [ ] 組織内のアカウントでCloutTrailをオフにしても、強制的にOnに戻す
    - Organizationと統合したCloudTrail + EventsでLamdba起動か
  - [ ] Configのルール違反を検知したら管理者にEメールとSlackで通知が届く
    - Slackに通知するにはLamdbaが必要かと思われる
    - Config + CloudWatchEvents + SNS + ladmbaとなるか?
    - [参考](https://aws.amazon.com/jp/premiumsupport/knowledge-center/sns-lambda-webhooks-chime-slack-teams/)
  - [ ] あらかじめ規定のリージョン以外でインスタンスが起動したらメールやSlackで管理者に通知する
    - CloudTrailで組織のログを確認 + CloudWatchEvents?
  - [ ] 承認されていないAMIでインスタンスが立ちあがった場合に管理者に通知するConfigルール
- IaCあれこれ
  - [ ] Lamdbaを効率的に管理
    - TerraFormはインフラの管理なのでちょっとアプリケーションコードもあるLamdbaは辛いか
  - [ ] TerraFormでEKSクラスターを管理したい
    - CKA・CKADの取得後にしたい

## DevOps関連

- [ ] Kubernetesを理解・客観的に実力を証明
  - [ ] CKAの取得
  - [ ] CKADの取得
