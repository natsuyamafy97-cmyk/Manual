# 1. クローン先に移動
cd ~          # ホームディレクトリ

cd projects   # プロジェクトフォルダがあればそこへ

# 2. Git Clone 実行

HTTPS の場合

git clone https://github.com/natsuyamafy97-cmyk/REPOSITORY.git

SSH の場合（SSHキーを設定済みならこちら推奨）

git clone git@github.com:natsuyamafy97-cmyk/REPOSITORY.git

# 3. クローン結果を確認
ls


例:

REPOSITORY/


中に入って確認:

cd REPOSITORY

git status


✅ これで GitHub 上のリポジトリがローカル（EC2やPC）にコピーされます！
