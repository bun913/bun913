
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
  - [x] ANS
  - [ ] DAS
  - [ ] MLS
- [x] CKA合格
- [x] CKAD合格


## DevOps関連やりたいこと

まずはk8sを学習しながらコンテナオーケストレーションのアーキテクチャを学習する。

またDevOpsの文化・思想を自分の中に落とし込んで、「ただツールが使える」エンジニアにならないように、自分がDevOpsの文化をチームに根付かせるための土台にする。

その後具体的なツールの学習を進める。

- [x] Kubernetesを理解・客観的に実力を証明
  - [x] CKAの取得
  - [x] CKADの取得
- [ ] DevOpsの文化を理解する
  - [ ] The Unicorn Projectをまとめながら読了
  - [ ] The DevOpsハンドブックをまとめながら読了
  - [ ] Effective DevOpsをまとめながら読了
- [ ] DevOpsに必要なツールを学習
↑未定

## AWS関連やりたいこと

AWS11冠を目指しながら学習する中で作ってみたいと思ったものをまとめ。
DevOpsの文化を抑えるのを優先する。

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
