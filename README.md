# GitHubActionsIntroduction

![Swift](https://github.com/hal-cha-n/GitHubActionsIntroduction/workflows/Swift/badge.svg)

このリポジトリは GitHub Actions の動作確認リポジトリです。

# 行ったこと

### 1. ワークフローを設定
ActionsタブよりSwiftのワークフローを選択しました
![d2537b4ccbf64d46432f7e1cd802ee70](https://user-images.githubusercontent.com/40711834/103928645-7dd84300-515f-11eb-9dcf-bcd9476add1a.png)

### 2. Swiftプロジェクト生成

以下のコマンドでSwiftのビルドに必要なファイルを作成しました。

```sh 
$ swift package init --type executable
```

### 3. プルリクエスト作成

動作確認用プルリクエスト作成しました
- [ビルドできないコードを追加](https://github.com/hal-cha-n/GitHubActionsIntroduction/pull/1)
- [テストが失敗するコードを追加](https://github.com/hal-cha-n/GitHubActionsIntroduction/pull/2)
- [テストが成功するコード追加](https://github.com/hal-cha-n/GitHubActionsIntroduction/pull/3)

### 4. Branch protection rule 設定

mainブランチの`Branch protection rule` に `Require status checks to pass before merging` を有効化しました。
この設定により、mainブランチへのプルリクエストはbuildのジョブが成功していることが必須となります。

![1db57fc83189ffc9f348159dabfe9236](https://user-images.githubusercontent.com/40711834/103929508-c3494000-5160-11eb-916e-6da0f197de16.png)

