# kaggle-docker-gpu

DockerでGPU利用可能なkaggle環境を構築

## Requirements


## Usage

```
$cd kaggle-docker-gpu
$sudo docker-compose up --build　# buildには1.5h~2hくらいかかる
# コンテナ入る
$sudo docker-compose exec kaggle-gpu bash
```


build後，localhost:9999にアクセスすると，jupyter labが起動している．

## Note
- mlflowとtensorboardのコンテナも用意してあるので，利用したい時はkaggle-docker-gpu直下に
artifact, mlruns, logsというフォルダを作る．その後，docker-compose.ymlのコメントアウトしてある部分を解除．
- 
