# 次にやりたいこと・作りたいもの(Next Challenge)

プライベートで達成したい目標・やりたいことを管理

## 年間目標(Annual Targets)

### 2022 年度

- [x] OSSのコントリビューターになる(Be a OSS contributer.)
  - 忙しくて最近できていないけど・・・
- [x] AWSとTerraformを利用したサービス構築業務をやり切る(Complete a service building work using AWS.)
- [ ] AWSのベータ版試験(AWS on SAP)が正式版になったら合格する(Pass the AWS beta exam when it becomes official.)
- [x] TOEICで600点を超える(Score over 600 on TOEIC.)
  - 初受験で605点!!1日10分くらいでも毎日続ければ力になる模様 
- [x] TOEICで650点を超える(Scored 675)
- ~~[ ] CCNA合格~~
- [ ] AtCoderで茶色になる

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

## AWS 関連やりたいこと

今年は技術面ではAWSによるサービス構築、Terraformによるコード化に力を入れる。

以下まずはハンズオンで学び、次はTerraformによる自動化まで行って完了とする。
また、極力zennなどに投稿し自身だけでなく誰かの学習にも役立てる様にすること。

- [シンプルなコンテナアプリをFARGATEで構築。BGデプロイまでTerraformで構築する](https://github.com/bun913/aws_network_practice/tree/main/simple_ecs_app)
- [プライベートサブネットのEC2にSSMで接続](https://github.com/bun913/aws_network_practice/tree/main/aurora)
- [CloudFrontに独自ドメイン設定。あえてDNSにRoute53を使わない](https://github.com/bun913/aws_network_practice/tree/main/cloudfront_s3_acm)
- [Terraformで機密情報を扱うには ~RDSパスワード編~](https://github.com/bun913/aws_network_practice/tree/main/aurora)
- [FARGATE実行環境のログをfluendのサイドカーで収集。Firehoseにストリーミングして、S3にも吐かせる。](https://github.com/bun913/aws_network_practice/tree/main/ecs_cloudwatch_logs)
    - CloudWacthLogsに出力するログはSlackとemail通知をしたい
- SSM AutomationによるEC2の夜間自動停止などの仕組みをTerraformで作る
- AWSの負荷テストソリューションで負荷テストを試したい
