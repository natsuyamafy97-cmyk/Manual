## 1. 新機能や修正のためのブランチを作成
git checkout -b feature-xxx

## 2. コードを修正 → コミット

git add .

git commit -m "Add xxx feature"

## 3. 動作確認して問題なければ main にマージ

git checkout main

git pull origin main   # 念のため最新化

git merge feature-xxx

## 4. リモートに反映
git push origin main

## 5. ブランチ削除（不要なら）

git branch -d feature-xxx

git push origin --delete feature-xxx   # GitHub側も消すなら

🔹 一人開発ならこんなパターンが便利

新機能ごとにブランチ → 完了したら main に取り込む

大きな修正のテスト → 別ブランチで試して問題なければマージ

短期的に使う実験 → 使い終わったらブランチ削除
