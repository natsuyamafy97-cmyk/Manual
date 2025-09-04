🔹 GitHub Desktop でのブランチ作業の流れ
## 1. ブランチを切り替える

GitHub Desktop を開く

左上の Current Branch をクリック

既存のブランチ一覧が出るので、作成済みのブランチを選択

👉 これでそのブランチの状態に切り替わります。

## 2. 修正をする

エディタ（VSCode など）でプロジェクトを開いて修正

変更すると GitHub Desktop の画面に 変更ファイル一覧 が表示されます

## 3. コミットする

GitHub Desktop 下部にある

Summary (コミットメッセージ)

Description (任意の詳細) を入力

Commit to <ブランチ名> をクリック

## 4. リモートに Push

上のメニューに Push origin ボタンが出るのでクリック
（または Ctrl + P でプッシュ）

## 5. main に取り込む

GitHub Desktop では、ブランチを main にマージするのはちょっと手間です。
方法は2つあります👇

A. GitHub Desktop で直接マージ

Current Branch → main に切り替える

メニューから
Branch → Merge into Current Branch を選択

マージしたいブランチを選んで実行

B. GitHub 上で Pull Request を作ってマージ

GitHub の Web 画面から「Pull Request」を作ってマージする方法

一人開発なら Desktop で直接マージの方が早いです
