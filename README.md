# docker rails template

to initialize from baseの通りで始めれば良い。

Railsのテンプレートは以下のGISTから読み込んでいる。
https://gist.githubusercontent.com/masashi-fuji/26e4f31397e39193dbf002a8b714ea38/raw/slim-rails.rb
Gemfileなどの初期設定を更新する時にはこのGISTを編集する。


## to initialize from base

```fish
git clone git@github.com:masashi-fuji/rails_docker_template.git
cd rails_docker_template
script/init; and script/bootstrap
```

## to bootstrap after clone

```fish
git clone git@github.com:masashi-fuji/rails_docker_template.git
cd rails_docker_template
git checkout -b ruby-2.4.0-rails-5.0.1 origin/ruby-2.4.0-rails-5.0.1; and script/bootstrap
```

## to develop

```bash
docker-compose up -d
docker-compose exec spring rails db:migrate
```

## License

MIT
