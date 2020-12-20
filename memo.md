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
開発用ブランチ作成