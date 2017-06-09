# docker rails template

## to initialize from base

```fish
git clone git@github.com:masashi-fuji/rails_docker_template.git
cd rails_docker_template
script/init; and script/bootstrap
```

## to bootstrap after clone

```fish
git clone https://github.com/kawasin73/rails_docker_template.git
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
