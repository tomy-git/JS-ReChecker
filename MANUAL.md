# 開発におけるDockerマニュアル

## 最初の立ち上げ（Docker Containerのビルド〜起動）
### 1.GitHubからこのリポジトリをcloneする
GitHubからクローンしてきてください。Dockerの起動に必要な設定ファイルはすべてコミットしてあります。

### 2.DockerのContainerをBuildする
1. ターミナルなどからこのクローンしてきたファイルのあるディレクトリに移動します。
2. 以下のコマンドを実行します。
`docker compose up -d --build`
これでPython3を扱える環境をすべて構築してくれます。

### 3.立ち上げたコンテナにログインする
以下のコマンドを実行することでコンテナにログインできます。
`docker compose exec python3 bash`

## コンテナの停止方法
`docker stop python3`

## コンテナの起動方法
`docker start python3`

## コンテナのログイン方法
`docker compose exec python3 bash`
