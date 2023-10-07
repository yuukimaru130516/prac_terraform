# Terraform 練習用リポジトリ

このリポジトリはTerraformの練習をするためのリポジトリです．システム構成と，ディレクトリ構成は以下のようになっています．

TODO：システム構成

## ディレクトリ構成

```
---- terraform
   │   └ src
   │   │   └ main.tf
   │   │   └ その他もろもろ // Terraform関連ソース(docker-composeでマウントする)
   │   └ home
   │   │   └ entrypoint.sh // TerraformコンテナのENTRYPOINTに指定するシェルコマンド
   │   └ root
   │   │   └ .bashrc // bashのエイリアスなどをここに記載
   │   └ Dockerfile
   └ docker-compose.yaml
```

## 環境構築

Dockerを用いて，実行環境の構築を行います．まず，`Dockerfile`が存在するディレクトリ内で，以下のコマンドを実行する．

```{bash}
docker compose up -d
```

