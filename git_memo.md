
# Git

実際の開発時によくやりそうなこと

開発用ブランチ作成→開発用ブランチにadd,commit→リモートにpush→作業用ローカルブランチを削除

事前：git cloneしておく

1. masterブランチから作業用ブランチを切る(ローカル)

   ```bash
   #ローカルに新規ブランチ作成
   git branch new_baranch

   #作成したブランチに切替
   git checkout new_branch
   ```

2. 作業完了したらリモートリポジトリにプッシュする(ローカル)

    ```bash
   #ファイルをステージング
   git add .
   git commit -m "こめんと"

   #リモートブランチに作業ブランチをpush
   git push origin new_baranch
   ```

3. リモートリポジトリでマージする

<br>

4. ローカルとリモートを同期する

    ```bash
    #branchをマスターに変更
    git checkout master
    #リモートリポジトリから最新の状態をプルする
    git pull origin master
    #不要なbranchを削除
    git branch -d new_branch
    ```

5. 覚えておくといいやつ

    ```bash
    #ローカルのブランチを確認する
    git branch
    #リモートブランチを確認する
    git remote
    #ローカルのブランチ切替
    git checkout '対象のブランチ'
    #ステージング状況を確認する
    git status    
    #リモートブランチの切替
    git xxx
    →使うか？
    #リモートブランチの削除
    git remote rm '対象のリモートブランチ'
    #リモートにブランチを登録する
    git push -u 'リモートブランチ名' '作成したブランチ名'
   ```

変更箇所などなにもない
変更箇所
変更箇所