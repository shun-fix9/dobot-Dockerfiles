# dobot 用 dockerfile

## elasticsearch-kuromoji

### ビルド方法

```bash
cd elasticsearch-kuromoji
docker build --rm -t sakai/dobot-elasticsearch-kuromoji:<tag> .
```

### 詳細

* kuromoji インストール済み


## node : node + ssh

### ビルド方法

```bash
cd node
docker build --rm -t sakai/dobot-node:<tag> .
```

### 詳細

以下が volume に設定してある

* /var/www/dobot
