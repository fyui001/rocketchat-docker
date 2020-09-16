# セットアップ

### サンプルからコピーしてdocker-compose.ymlを適宜書き換える

```
cp docker-compose-example.yml docker-compose.yml
```
### 先にmongoだけ起動させる

```
docker-compose up -d mongo
```
### logs監視してmongoが完全に起動するまで待つ

```
docker-compose logs -f
```

### mongo-initを立ち上げてmongoのレプリカを初期化

```
docker-compose up -d mongo-init
```

### 最後にrocketchatを立ち上げておわり

```
docker-compose up -d rocketchat
```
