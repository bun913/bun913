# 次にやりたいこと・作りたいもの

プライベートで達成したい目標・やりたいことを管理

## 年間目標

### 2021 年度

- [x] AWS 認定試験 11 種合格
  - [x] DVA
  - [x] SAP
  - [x] DOP
  - [x] SCS
  - [x] DS
  - [x] ANS
  - [x] DAS
  - [x] MLS
- [x] CKA 合格
- [x] CKAD 合格

## DevOps 関連やりたいこと

まずは k8s を学習しながらコンテナオーケストレーションのアーキテクチャを学習する。

また DevOps の文化・思想を自分の中に落とし込んで、「ただツールが使える」エンジニアにならないように、自分が DevOps の文化をチームに根付かせるための土台にする。

その後具体的なツールの学習を進める。

- [x] Kubernetes を理解・客観的に実力を証明
  - [x] CKA の取得
  - [x] CKAD の取得
- [x] DevOps の文化を理解する
  - [x] The Unicorn Project をまとめながら読了
  - [x] The DevOps ハンドブックをまとめながら読了
  - [x] Effective DevOps をまとめながら読了
- [x] DevOps に必要なツールを学習
   - [この本](https://www.amazon.co.jp/dp/B09DKZC1ZH/ref=dp-kindle-redirect?_encoding=UTF8&btkr=1)を使って terraformに置き換えながらハンズオンで学習
- [x] ユニットテストの知見を広げたい（コードの品質を上げて、心理的安全性を高めることができるようになりたい）
  - [やってみたリポジトリ](https://github.com/bun913/software_test_practice_go)

## 関数型プログラミングを理解する

- [ ] 楽しいHaskell本をやってみる

## AWS 関連やりたいこと

AWS11 冠を目指しながら学習する中で作ってみたいと思ったものをまとめ。
DevOps の文化を抑えるのを優先する。

作成したらリポジトリのリンクを随時貼っていきます。

- EC2 あれこれ
  - [x] 平日の深夜や土日に特定のタグが付与された EC2 インスタンスを停止する
    - CloudWatchEvents + Lambda でスケジューリング実行
    - [やってみたリポジトリ](https://github.com/bun913/lamdba_ec2_stop)
  - [X] 上に関連して特定のタグが付与された EC2 インスタンスを毎朝起動する
    - CloudWatchEvents + Lambda でスケジューリング実行
      - ついでにGithubActionsを使ってみた 
    - [やってみたリポジトリ](https://github.com/bun913/ec2_auto_start)
- StepFunctions / lambdaあれこれ
  - [ ] S3イベント通知 -> StepFunction で EC2の処理を実施 -> 結果をSlackで通知 したい
- セキュリティ・コンプライアンス
  - [ ] 組織内のアカウントで CloutTrail をオフにしても、強制的に On に戻す
    - Organization と統合した CloudTrail + Events で Lamdba 起動か
  - [ ] Config のルール違反を検知したら管理者に E メールと Slack で通知が届く
    - Slack に通知するには Lamdba が必要かと思われる
    - Config + CloudWatchEvents + SNS + ladmba となるか?
    - [参考](https://aws.amazon.com/jp/premiumsupport/knowledge-center/sns-lambda-webhooks-chime-slack-teams/)
  - [ ] あらかじめ規定のリージョン以外でインスタンスが起動したらメールや Slack で管理者に通知する
    - CloudTrail で組織のログを確認 + CloudWatchEvents?
  - [ ] 承認されていない AMI でインスタンスが立ちあがった場合に管理者に通知する Config ルール
- IaC あれこれ
  - [ ] Lamdba を効率的に管理
    - TerraForm はインフラの管理なのでちょっとアプリケーションコードもある Lamdba は辛いか
  - [ ] TerraForm で EKS クラスターを管理したい
    - CKA・CKAD の取得後にしたい
