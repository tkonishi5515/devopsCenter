---
title: DevOpsCenter について
marp: true
paginate: true
theme: freud
---

<!-- _paginate: false -->
<!-- theme: gradient class: blue-->
<!-- theme: freud class: blue-->

# DevOpsCenter について <!-- fit -->

</br>
</br>

![Slides are here](images/qrcode.png)

##### スライド:https://tkonishi5515.github.io/devopsCenter/ja/index

##### リポジトリ:https://github.com/tkonishi5515/devopsCenter

---

# 初めに

- 深い箇所まで実践できていないため、現時点で私が理解している箇所を共有いたします
- 詳細な設定方法は説明しません

---

# トピックス

1. DevOpsCenter とは？
2. DevOpsCenter でできること
3. DevOpsCenter と変更セット
4. DevOpsCenter の触り
5. 実践

---

# DevOps とは

- ソフトウェア開発（Development）と IT 運用（Operations）の間のコラボレーションや統合を促進する一連の実践と哲学のことです
- 開発と運用の両チームが一緒に働く文化やプロセスのことです
- 利便性を高めたい開発者と、安定的な運用をしたい運用者との間で、対立が生じた際に生まれました。
  ![height:200](images/1.webp)

---

# DevOps Center とは

- 2022 年 12 月に正式リリース

- [Trailhead](https://trailhead.salesforce.com/ja/content/learn/modules/devops-center-quick-look/say-hello-to-devops-center?trailmix_creator_id=jimsharp&trailmix_slug=learn-dev-ops-center)に簡単に記載されている
- 恐ろしいことに「変更セットが気に入っている場合は、心配しないでください。現時点では廃止されません。」と記載されています

  - 将来的に変更セットを廃止する予定？

- [構成](https://help.salesforce.com/s/articleView?id=sf.devops_center_configure.htm&type=5)など設定方法は記載されているので、興味がある方は確認してみてください。

---

# DevOpsCenter でできること

- タスクの管理
  - DevOpsCenter 上でタスク(チケット)を作成し、成果物と結びつけることができる
- レビュー機能
  - GitHub と連携しているため、差分の確認が楽
  - 特に Apex や LWC を使用するプロジェクトでは、すごく楽になる
- リリース機能
  - ステージング環境や UAT 環境を設定しておき、修正した内容をリリースすることができる
  - 環境をメタデータで管理するため、デグレが起きにくい

---

# DevOpsCenter と変更セット

- 相違点
  - ブランチ単位で管理ができるため DevOpsCenter はデグレが起きにくい
  - 開発環境で修正した箇所を自動で表示してくれるため、リリース漏れが起きにくい
  - GitHub 上でレビュー(PullRequest)をできるためレビューする人も簡単

---

# DevOpsCenter を行う際に必要なもの

- GitHub
  - 今回は個人のアカウントで行なっていますが、本格的に行いたい場合は会社で契約する必要あり
  - GitLab や BackLog の連携は今の所不可(BackLog 連携はシェア率的に厳しそう)
- Salesforce DX
  - 事前に設定しておく必要あり
- ブランチ戦略
  - プロジェクトが始まる前に用意しておくと良さそう

---

# DevOpsCenter を行う際に必要ないもの

- vsCode
  - 画面上でリリースや、マージを行うことができるため vsCode の設定は不要

---

# 使用するイメージ

- 画像貼り付ける

---

# 実践

---

# まとめ

- Aura と LWC の違いはさまざまあるが、基本 LWC を使用しよう
- 画面フローで実装可能な場合は、画面フローで実装しよう
