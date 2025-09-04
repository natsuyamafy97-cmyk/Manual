## 1. 作業中の変更状況確認

### 1-1. ステージしていない変更を確認
git diff

### 1-2. ステージ済みの変更を確認
git diff --cached

### 1-3. 最新コミットとの差分確認
git diff HEAD

ステージ済み・未ステージ両方の差分を確認可能

## 2. ステージング（コミット対象に追加）
特定ファイルをステージする場合

git add ファイル名

作業ディレクトリ全体をステージする場合

git add .

ステージ状態を確認

git status

Changes to be committed にファイルが表示されればOK

## 3. 再度差分を確認（オプション）
git diff --cached


ステージ済み差分のみを確認

## 4. コミット
コミットコマンド
git commit -m "Add login feature and update README"

コミットメッセージのポイント

何を変更したか明確に書く

過去形で簡潔にまとめる

複数の変更がある場合は別コミットに分ける

## 5. リモートへのプッシュ
プッシュコマンド
git push origin main

SSH接続の場合
git push git@github.com:ユーザー名/リポジトリ名.git

## 6. コミット確認
git log --oneline
