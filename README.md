docker compose up -d


docker-compose run web django-admin startproject 'app' .

python manage.py runserver

### python

python

### pip 使えるように

python -m pip install pillow

## その他コマンド

イメージ全削除
docker rmi $(docker images -q) -f

コンテナ全削除
docker rm $(docker ps -a -q) -f

不要物一括削除
docker system prune

再ビルド キャッシュ削除
docker-compose build --no-cache