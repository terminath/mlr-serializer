# Machine Learning Regularly Serializer

機械学習の学習済みモデルのインスタンスを定期的にシリアライズする装置。  
機械学習をバッチで動かし、学習結果をファイル出力。

## Requires
- Python 3.x
- Pipenv

## Installing
以下コマンドで依存関係のインストールをする。
```
pipenv install
```

## Backend
サンプルの Django バックエンドサーバーを作成済み。  
このサーバーで機械学習を行う。 

サーバーの起動
```
pipenv run start_back
```

## Job Scheduler
以下のコマンドでジョブスケジューラのサーバーを構築、起動。
```
docker-compose up -d job
```

## Servers
本システムで予め用意しているサーバーは以下の通り。

| Server | Host | Port |
| --- | --- | --- |
| mlr_backend | 127.0.0.1 | 8765 |