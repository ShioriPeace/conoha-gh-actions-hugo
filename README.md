# conoha-gh-actions-hugo
http://hayapi.conohawing.com/


## 作成するファイル
ファイル名：`（会社名）（社員番号）（名前）.md`

```
---
title: "（会社名）（社員番号）（名前）"
date: 2020-05-07T02:00:04+09:00
draft: false
---

## 自己紹介
- 会社名
- 社員番号
- 名前

```

### 開発の流れ

1. リポジトリをローカルマシンにclone
```
git clone git@github.com:hayasaki-shunsuke/conoha-gh-actions-hugo.git
cd conoha-gh-actions-hugo
```
2. ローカルで修正用ブランチを切る
```
git checkout -b pepabo-hayasaki
```
3. `（会社名）（社員番号）（名前）.md`を作成
```
hugo new content/posts/pepabo-552-hayasaki.md
```
4. 内容を修正する
```text:sample
---
title: "（会社名）（社員番号）（名前）"
date: 2020-05-07T02:00:04+09:00
draft: false
---

## 自己紹介
- 会社名
- 社員番号
- 名前
```
5. 修正をcommitして、ブランチをGitHubにpushする
```
git add content/posts/pepabo-552-hayasaki.md
git commit -m "hayasakiのファイルを追加"
```
6. GitHub上でPull Requestを作成する
7. レビューを依頼する
8. レビューがOKならmasterブランチにmergeする
9.  [本番環境](http://hayapi.conohawing.com/)で確認する
