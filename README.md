# WordPressBaseTheme
- Docker
- SCSS
- webpack

# 必須環境
- Docker
- Node.js
- npm

# 環境構築

### npmインストール

```
npm install
```

または

```
make npm
```

### Dockerコンテナのビルド

```
docker compose up -d
```

または

```
make up
```

# 使用方法

```
npm run dev
```

を実行し、CLIにエラーが発生しなければ通常に起動します。



Windows + WSL2環境の場合permission deniedエラーが発生する場合があるが、

Dockerコンテナの初回ビルド時にdistファイルがroot権限で生成されるため。

修正する際はWSL2内で、

```
sudo chown {ユーザーネーム}:{ユーザーグループ} dist
```

を実行します。
