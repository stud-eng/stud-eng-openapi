# stud-eng-openapi
stud-eng-apiのAPI仕様書を作成するためOSAで実装する。
npmコマンドが実行可能な環境を準備してください
[document](https://docs.npmjs.com/)
## インストール方法
`$ npm i -g @redocly/cli@latest`

## ドキュメント作成方法
1. yamlファイルの構文チェック
```
$ redocly lint openapi.yaml
```

2. ドキュメント作成
```
$ redocly preview-docs openapi.yaml
```
出力されたURLにアクセスしてドキュメントを確認する。

3. ドキュメント用のHTMｌファイルを作成
```
$ redocly build-docs openapi.yaml
```
redoc-static.html ファイルが作成されるのでファイルのパスを指定して
ブラウザからドキュメントを閲覧する。