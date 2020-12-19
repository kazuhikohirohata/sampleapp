# Pythonの学習フロー

---

## 事前準備

- pythonのインストール
- GitHubアカウントの作成
- VScodeで色々書いてみる(UML,Markdown)

## 学習の流れ

1. progateでガチャガチャやってみる
2. ローカルで書いてみる
3. GitHubアカウントにぶちこむ

```puml

(*) --> "pythonでなんか書く"
partition loop {
"pythonでなんか書く" --> "Githubにコミット、プッシュ"
"Githubにコミット、プッシュ" --> "プルリク"
}
"プルリク" --> "確認"
```

- Djyangoの参考サイトは[ここ](https://docs.djangoproject.com/ja/3.1/intro/tutorial01/)がよさそう
- つづけてみる

##　学習メモ

- アノテーション
→コードの注釈(@xxxxのような感じ)

## Git

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

4. ローカルとリモートを同期する

    ```bash
    #branchをマスターに変更
    git checkout master
    #リモートリポジトリから最新の状態をプルする
    git pull origin master
    #不要なbranchを削除
    git branch -d new_branch
    ```
