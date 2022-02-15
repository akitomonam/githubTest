# Git学習メモ
## Gitコマンド

ローカルリポジトリの作成
```
git init
```
ファイル状態の確認
```
git status
```
ファイルの登録
```
git add
```
ファイルの退避
```
git stash
```
### ローカルリポジトリをリモートリポジトリに登録
まず，ローカルリポジトリに移動

ローカルリポジトリはコミット済みにしておく

リモートリポジトリを追加
```
git remote add <remote name> <remote URL>
```
＊\<remote URL\>はベアリポジトリ
カレントのブランチ名をbranch nameに変更
```
git branch -M <branch name>
```
リモートに現在のリポジトリをプッシュ
```
git push -u <remote name> <branch name>
```
### 作業ブランチをメインブランチで最新化
```
git checkout branch_name
git merge main
```
### 最終コミットの戻す
```
git reset --hard HEAD
```
