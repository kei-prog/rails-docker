# 環境構築手順
```
git clone https://github.com/kei-prog/rails-docker.git

cd rails-docker

docker compose up -d

docker-compose run web rake db:create

docker-compose run web rails db:migrate RAILS_ENV=development

docker-compose run web rails webpacker:install

# localhost:3000にアクセスできればOK

```

