# Git 基本操作まとめ

## 1. リポジトリの作成

### ローカルで新規作成
```bash
cd プロジェクトフォルダ
git init
```

### 既存リモートリポジトリをクローン
git clone <リポジトリURL>

## 2. ファイルの状態確認
git status


Untracked files: Git管理対象外

Changes not staged for commit: 変更があるがステージしていない

Changes to be committed: ステージ済みでコミット可能

## 3. 変更のステージング
git add ファイル名       * 個別追加

git add .               * 全て追加

## 4. コミット

git commit -m "コミットメッセージ"

## 5. リモート操作

リモート設定確認

git remote -v

プッシュ（リモートに反映）

git push origin ブランチ名

プル（リモートから取得）
git pull origin ブランチ名

## 6. ブランチ操作
作成

git branch ブランチ名

切替

git checkout ブランチ名

作成＋切替

git checkout -b ブランチ名

## 7. 不要なファイルをGit管理外にする
### 1. .gitignore に追加
echo "フォルダ名/" >> .gitignore
git add .gitignore
git commit -m "Ignore フォルダ名"

### 2. 既に管理されている場合はキャッシュ削除
git rm -r --cached フォルダ名
git commit -m "Remove フォルダ名 from git tracking"

## 8. 変更差分の確認
git diff            # ステージしていない差分
git diff --staged   # ステージ済みの差分

