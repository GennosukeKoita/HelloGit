# 超基本！！
## Github上でNewを押して、レポジトリを作成

# gitの初期設定
> ユーザ名を設定
git config —global user.name “ユーザ名”
git config ―global user.email “メールアドレス”

> ローカルレポジトリを作成
mkdir ファイル名
cd ファイル名
git init

> ローカルレポジトリにファイルの変更点を追加
git add ファイル名

> ローカルレポジトリにインデックスに追加したファイルを追加
git commit -m “何をしたのか記入（例）変更したとかver 1.0とか”


> 追加したインデックスをGithubに作成
git remote add origin ユーザID名(CodeのHTTPSをコピーすればいい)

> ローカルレポジトリのファイルをGithubのレポジトリに送信
git push -u origin master

# プッシュしたデータを変更・更新してみる

> 変更をインデックスに追加
git add ファイル名

> ファイルを登録
git commit -m “何をしたのか送信”

> データの送信
git push -u origin master

# ブランチを作る（一気にバージョンを作成するとき、失敗した時用に作っておくようなもの）

> ブランチの作成
git branch ブランチ名

> 今あるブランチを確認する
git branch

> 参照や書き換え先のブランチをブランチ名に変更する場合
git checkout ブランチ名

# 作ったブランチにデータを送信

> 変更をインデックスに追加
git add ファイル名

> ファイルを登録
git commit -m “何をしたのか送信”

> Githubにローカルレポジトリのデータを送信（プッシュする）
git push origin ブランチ名

# ブランチを本筋に統合する

> 取り込み先のブランチを選択する
git checkout master

> masterにブランチ名を統合する
git merge ブランチ名

> 結合情報をGithubに送信する
git push -u origin master